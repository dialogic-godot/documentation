
<div class="header-banner purple">
<div class="header-label purple">Save</div>
</div>

*This contains the source code documentation of the class `subsystem_Save`.*
        
# subsystem_Save
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem to save and load game states.
## Description
This subsystem has many different helper methods to save Dialogic or custom game data to named save slots.  You can listen to saves via [saved](#signal-saved). \ If you want to save, you can call [save](#property-save). \

## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">autosave_enabled</span>](#property-autosave_enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">autosave_mode</span>](#property-autosave_mode) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">autosave_time</span>](#property-autosave_time) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `60` 
[<span class="hljs-title">autosave_timer</span>](#property-autosave_timer) | [Timer](https://docs.godotengine.org/en/latest/classes/class_timer.html#class-timer) |   
[<span class="hljs-title">latest_thumbnail</span>](#property-latest_thumbnail) | [Image](https://docs.godotengine.org/en/latest/classes/class_image.html#class-image) |  `null` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">add_empty_slot</span>](#method-add_empty_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">delete_slot</span>](#method-delete_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_default_slot</span>](#method-get_default_slot) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_encryption_password</span>](#method-get_encryption_password) ( ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">get_global_info</span>](#method-get_global_info) ( `key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_latest_slot</span>](#method-get_latest_slot) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_slot_info</span>](#method-get_slot_info) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[String[]](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_slot_names</span>](#method-get_slot_names) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_slot_path</span>](#method-get_slot_path) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[ImageTexture](https://docs.godotengine.org/en/latest/classes/class_imagetexture.html#class-imagetexture)</span> | [<span class="hljs-title">get_slot_thumbnail</span>](#method-get_slot_thumbnail) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_slot</span>](#method-has_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">load</span>](#method-load) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">load_file</span>](#method-load_file) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `file_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">perform_autosave</span>](#method-perform_autosave) ( ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">reset_slot</span>](#method-reset_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">save</span>](#method-save) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `is_autosave`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `thumbnail_mode`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `1`, `slot_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">save_file</span>](#method-save_file) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `file_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `data`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">save_slot_thumbnail</span>](#method-save_slot_thumbnail) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">set_global_info</span>](#method-set_global_info) ( `key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">set_latest_slot</span>](#method-set_latest_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">set_slot_info</span>](#method-set_slot_info) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">take_thumbnail</span>](#method-take_thumbnail) ( ) 
--- 
## Constants


<a class="header" id="constant-SAVE_SLOTS_DIR" href="#constant-SAVE_SLOTS_DIR">**<span class="hljs-attribute">const</span> <span class="hljs-title">SAVE_SLOTS_DIR</span><span class="hljs-comment"> = "user://dialogic/saves/"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-AUTO_SAVE_SETTINGS" href="#constant-AUTO_SAVE_SETTINGS">**<span class="hljs-attribute">const</span> <span class="hljs-title">AUTO_SAVE_SETTINGS</span><span class="hljs-comment"> = "dialogic/save/autosave"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-AUTO_SAVE_MODE_SETTINGS" href="#constant-AUTO_SAVE_MODE_SETTINGS">**<span class="hljs-attribute">const</span> <span class="hljs-title">AUTO_SAVE_MODE_SETTINGS</span><span class="hljs-comment"> = "dialogic/save/autosave_mode"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-NONE" href="#constant-NONE">**<span class="hljs-attribute">const</span> <span class="hljs-title">NONE</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TAKE_AND_STORE" href="#constant-TAKE_AND_STORE">**<span class="hljs-attribute">const</span> <span class="hljs-title">TAKE_AND_STORE</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-STORE_ONLY" href="#constant-STORE_ONLY">**<span class="hljs-attribute">const</span> <span class="hljs-title">STORE_ONLY</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ON_TIMELINE_JUMPS" href="#constant-ON_TIMELINE_JUMPS">**<span class="hljs-attribute">const</span> <span class="hljs-title">ON_TIMELINE_JUMPS</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ON_TIMER" href="#constant-ON_TIMER">**<span class="hljs-attribute">const</span> <span class="hljs-title">ON_TIMER</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ON_TEXT_EVENT" href="#constant-ON_TEXT_EVENT">**<span class="hljs-attribute">const</span> <span class="hljs-title">ON_TEXT_EVENT</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-saved" href="#signal-saved">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">saved</span>](#signal-saved) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 Emitted when a save happened with the following info: 
Key           |   Value Type  | Value 
-----------   | ------------- | ----- 
`slot_name`   | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) | The name of the slot that the game state was saved to. 
`is_autosave` | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)   | `true`, if the save was an autosave. 
 

---

## Property Descriptions



<a class="header" id="property-autosave_enabled" href="#property-autosave_enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">autosave_enabled</span> <span style = "color: gray"> = </span> false** 



Whether the auto-save feature is enabled. The initial value can be set in the project settings via th Dialogic editor.  This can be toggled during the game.

---



<a class="header" id="property-autosave_mode" href="#property-autosave_mode">**<span class="hljs-attribute">var</span> <span class="hljs-title">autosave_mode</span> <span style = "color: gray"> = </span> 0** 



Under what conditions the auto-save feature will trigger if `autosave_enabled` is `true`.

---



<a class="header" id="property-autosave_time" href="#property-autosave_time">**<span class="hljs-attribute">var</span> <span class="hljs-title">autosave_time</span> <span style = "color: gray"> = </span> 60** 



After what time interval the auto-save feature will trigger if `autosave_enabled` is `true` and `autosave_mode` is `AutoSaveMode.ON_TIMER`.

---



<a class="header" id="property-autosave_timer" href="#property-autosave_timer">**<span class="hljs-attribute">var</span> <span class="hljs-title">autosave_timer</span> <span style = "color: gray"> = </span> <unknown>** 



################################################################################################## Reference to the autosave timer.

---



<a class="header" id="property-latest_thumbnail" href="#property-latest_thumbnail">**<span class="hljs-attribute">var</span> <span class="hljs-title">latest_thumbnail</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-add_empty_slot" href="#method-add_empty_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_empty_slot</span>](#method-add_empty_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



This adds a new save folder with the given name

---



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Built-in, called by DialogicGameHandler.

---



<a class="header" id="method-delete_slot" href="#method-delete_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">delete_slot</span>](#method-delete_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



Removes all the given slot along with all it's info/files.

---



<a class="header" id="method-get_default_slot" href="#method-get_default_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_default_slot</span>](#method-get_default_slot) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the default slot name defined in the dialogic settings

---



<a class="header" id="method-get_encryption_password" href="#method-get_encryption_password">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_encryption_password</span>](#method-get_encryption_password) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Gets the encryption password from the project settings if it has been set. If no password has been set, an empty string is returned.

---



<a class="header" id="method-get_global_info" href="#method-get_global_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_global_info</span>](#method-get_global_info) ( `key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



Access the data unrelated to a save slot. First, the data must have been set with [set_global_info](#property-set_global_info).

---



<a class="header" id="method-get_latest_slot" href="#method-get_latest_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_latest_slot</span>](#method-get_latest_slot) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the latest slot or empty if nothing was saved yet

---



<a class="header" id="method-get_slot_info" href="#method-get_slot_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_slot_info</span>](#method-get_slot_info) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_slot_names" href="#method-get_slot_names">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_slot_names</span>](#method-get_slot_names) ( )</a>  ⇒ <span class="hljs-attribute">[String[]](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



################################################################################################## Returns a list of all available slots. Useful for iterating over all slots, e.g., when building a UI with all save slots.

---



<a class="header" id="method-get_slot_path" href="#method-get_slot_path">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_slot_path</span>](#method-get_slot_path) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the full path to the given slot folder

---



<a class="header" id="method-get_slot_thumbnail" href="#method-get_slot_thumbnail">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_slot_thumbnail</span>](#method-get_slot_thumbnail) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[ImageTexture](https://docs.godotengine.org/en/latest/classes/class_imagetexture.html#class-imagetexture)</span>** 



Returns the thumbnail of the given slot.

---



<a class="header" id="method-has_slot" href="#method-has_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_slot</span>](#method-has_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns true if the given slot exists.

---



<a class="header" id="method-load" href="#method-load">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load</span>](#method-load) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



Loads all info from the given slot in the DialogicGameHandler (Dialogic Autoload). If no slot is given, the default slot is used. To check if something is saved in that slot use has_slot(). If the slot does not exist, this method will fail.

---



<a class="header" id="method-load_file" href="#method-load_file">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_file</span>](#method-load_file) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `file_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



Loads a file using `slot_name` and returns the contained info.  This method allows you to build your own save and load system. You may be looking for the simple [load](#property-load) method to load the game state.

---



<a class="header" id="method-perform_autosave" href="#method-perform_autosave">**<span class="hljs-attribute">func</span> [<span class="hljs-title">perform_autosave</span>](#method-perform_autosave) ( )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



Perform an autosave. This method will be called automatically if the auto-save mode is enabled.

---



<a class="header" id="method-reset_slot" href="#method-reset_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset_slot</span>](#method-reset_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



Reset the state of the given save folder (or default)

---



<a class="header" id="method-save" href="#method-save">**<span class="hljs-attribute">func</span> [<span class="hljs-title">save</span>](#method-save) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `is_autosave`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `thumbnail_mode`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `1`, `slot_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



Saves the current state to the given slot. If no slot is given, the default slot is used. You can change this name in the Dialogic editor. If you want to save to the last used slot, you can get its slot name with the [method get_latest_slot()] method.

---



<a class="header" id="method-save_file" href="#method-save_file">**<span class="hljs-attribute">func</span> [<span class="hljs-title">save_file</span>](#method-save_file) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `file_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `data`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



Saves a variable to a file in the given slot.  Be aware, the `slot_name` will be used as a filesystem folder name. Some operating systems do not support every character in folder names. It is recommended to use only letters, numbers, and underscores.  This method allows you to build your own save and load system. You may be looking for the simple [save](#property-save) method to save the game state.

---



<a class="header" id="method-save_slot_thumbnail" href="#method-save_slot_thumbnail">**<span class="hljs-attribute">func</span> [<span class="hljs-title">save_slot_thumbnail</span>](#method-save_slot_thumbnail) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



No need to call from outside. Used to store the latest thumbnail to the given slot.

---



<a class="header" id="method-set_global_info" href="#method-set_global_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_global_info</span>](#method-set_global_info) ( `key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



Data set in global info can be accessed unrelated to the save slots. For instance, you may want to store game settings in here, as they affect the game globally unrelated to the slot used.

---



<a class="header" id="method-set_latest_slot" href="#method-set_latest_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_latest_slot</span>](#method-set_latest_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_slot_info" href="#method-set_slot_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_slot_info</span>](#method-set_slot_info) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-take_thumbnail" href="#method-take_thumbnail">**<span class="hljs-attribute">func</span> [<span class="hljs-title">take_thumbnail</span>](#method-take_thumbnail) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



This method creates a thumbnail of the current game view, it allows to save the game without having the UI on the save slot image. The thumbnail will be stored in `latest_thumbnail`.  Call this method before opening your save & load menu. After that, call [save](#property-save) with [constant ThumbnailMode.STORE_ONLY]. The [save](#property-save) will automatically use the stored thumbnail.

---

