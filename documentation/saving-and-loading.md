<div class="header-banner dawn">
     <div class="header-label dawn">Saving & Loading</div>
</div>

*Obviously, many games require the ability to save and load!*

## 📜 Content
[toc]

## 1. Built-in Saving

The saving subsystem allows you to save and load Dialogic timeline states, game thumbnails (screenshots), and extra information to Savegame slots. \
You want to save the player position or the last seen text? The built-in save system has it all covered!

Be aware that Savegames uses their name as a folder name; operating systems restrict the allowed characters for folder names.
It's recommended to rely on the Latin alphabet, numbers, and underscores.

If you don't care about Savegame slots, you can do the following:

```gdscript
# Example signal handling.
func _on_save_game_button_pressed() -> void:
    Dialogic.Save.save()

func _on_load_game_button_pressed() -> void:
    Dialogic.Save.load()
```

However, these methods will take screenshots too, which may affect performance slightly.\
If you want to prevent this from happening, it gets a bit more verbose:

```gdscript
# Example signal handling.
func _on_save_game_button_pressed() -> void:
    Dialogic.Save.save("", false, Dialogic.Save.ThumbnailMode.NONE)

func _on_load_game_button_pressed() -> void:
    Dialogic.Save.load("", false, Dialogic.Save.ThumbnailMode.NONE)
```


### 1.1 Take a thumbnail

If you would like to use thumbnails per Savegame slot, it's recommended to take the screenshot before opening your *Save & Load* layer. \
This can be achieved by calling `Dialogic.Save.take_thumbnail()` *before* you show the layer; for instance, in the button signal connection, open the layer.

If you go this route, you need to instruct the `Dialogic.Save.save(...)` method to *store only* and *not* take a screenshot.

```gdscript
Dialogic.Save.save(slot_name_variable, false, Dialogic.Save.ThumbnailMode.STORE_ONLY, slot_extra_info)
```

This snippet will automatically take the thumbnail saved at `Dialogic.Save.last_thumbnail` and use it.

## 1.2 Saving Extra Info

By default, Savegames contain information about Dialogic's timeline only. If you want to store specific information, we can achieve this by using `Dialogic.Save.set_slot_info(slot_name:String, info: Dictionary)` and `Dialogic.Save.get_slot_info(slot_name: String)` methods. \
However, the `Dialogic.Save.save(...)` method can simplify our work and skip calling the set method.

In the following code snippet, we will save the last used text line and the current time as extra information.

```gdscript
var extra_info := {}
extra_info["text"] = Dialogic.current_state_info["text"]
extra_info["date"] = Time.get_datetime_string_from_system(false, true)

Dialogic.Save.save(slot_name, false, Dialogic.Save.ThumbnailMode.STORE_ONLY, extra_info)
```

### 1.3 Global data

The simple approach to store your game data slot-indepently is to use the `Dialogic.Settings` subsystem.\
You can directly store the information on it:
```gdscript
Dialogic.Settings.text_speed = 0.05
```

On save, the data will be automatically stored into the global save file

However, if you want to write to the global save file directly, you can use the `Dialogic.Save` subsystem:
```gdscript
func set_player_name(name: String) -> void:
    # Setting a name for the key `player_name`.
    Dialogic.Save.set_global_info("player_name", name)
```

There is no rule for the global info `key`'s value; being consistent is good, though.

If you are interested in storing the history of visited text, take a look at the next chapter.


### 1.4 Saving Visited Events

When you play a visual novel and use multiple saves, you may find yourself discovering texts you already read, even on entirely different story branches. \
By default, Dialogic does *not* save the events players have already visited; however, there are two main ways to get it working.

1. The first approach is via the Dialogic Editor. Head to the `Settings` tab and select `History`. From here on, you can decide if you want the already-visited events must auto-save.\

2. This approach is a bit different: The following snippet will manually save the history to a file.
Use this in case the player reached the end of the game (credits?) and you want to ensure that the visited-events are
properly updated a last time.

```gdscript
var slot_name := "slot-3-page-2"

func _save_game() -> void:
     Dialogic.History.save_visited_history()
     Dialogic.Save.save(slot_name)

func _load_game() -> void:
     Dialogic.History.load_visited_history()
     Dialogic.Save.load(slot_name)

func _reset_visited_history() -> void:
     Dialogic.History.reset_already_visited_history()
```

If you prefer to set the configuration via code, take a look at the following snippet:

```gdscript
func _ready() -> void:
    Dialogic.History.save_already_visited_history_on_save = true
    Dialogic.History.save_already_visited_history_on_autosave = true
```

The example values will cause the visited event history to automatically save
on Auto-Save and normal Saves.



# 2. Handling Savegame Slots

A save game slot is identified by its slot name, a unique word that you, as a developer, decide.\
One way to name the slots could be by their index and the current save game page (if you intend to have many save games). This could result in slots named `slot_3_page_4`.

# 2.1 Check if a Savegame Slot exists

When you create your own save/load layer, you may want to check whether any of these slots even exist.

```gdscript
func load_save_game_slot(slot_name: String) -> void:
    if Dialogic.Save.has_slot(slot_name):
        # Do your logic...
```

However, you may also use `Dialogic.Save.add_empty_slot(slot_name: String)` and populate the missing slots. If you check using the snippet, it's not necessary at all, though.

# 2.2 Delete a Savegame Slot

You can delete a save game slot by using the `Dialogic.Save.delete_slot(slot_name: String)` method.


# 3. Manual Saving

If you want to roll your own save and load system, you can use `Dialogic.get_full_state() -> Dictionary` to get the state of Dialogic and then continue saving it the way you want to.\
Once you are read to load the data back, you will have to use `Dialogic.load_full_state(state: Dictionary)` to get your data back into Dialogic.

Overall, it's better to have an idea *why* you want to do manual saving and take inspiration from Dialogic's `save` and `load` methods.\
There is a chance, that Dialogic already supports your specific loading and saving requirements.
