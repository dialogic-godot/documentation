<div class="header-banner pineapple">
     <div class="header-label pineapple">Signals & Signal Events</div>
</div>

*Dialogic provides a lot of signals that allow you to react to all kinds of things.
If you are new to Godot's signals [learn how to use them here](https://docs.godotengine.org/en/stable/getting_started/step_by_step/signals.html).*

*In other programs, signals are often referred to as events, and they are a way to implement the [Observer pattern](https://en.wikipedia.org/wiki/Observer_pattern).*

## 📜 Content
[toc]

## 1. Signal event

The signal event is used to inform code outside Dialogic that something happened or should happen.

When reached, the event will emit the signal `Dialogic.signal_event` and pass along the argument given in the event.

![grafik](media/signal_event.png)

*Here the argument is `"activate_something"`.*

To react to the signal event, connect to it before starting your dialog:

```gdscript
func _ready():
     Dialogic.signal_event.connect(_on_dialogic_signal)

func _on_dialogic_signal(argument:String):
    if argument == "activate_something":
        print("Something was activated!")
```

---

## 2. Text signal

When using the `[signal=activate_something]` text effect, dialogic will emit the `Dialogic.text_signal` signal with the given argument.

You can connect it the same way as the signal_event signal:

```gdscript
func _ready():
     Dialogic.text_signal.connect(_on_dialogic_text_signal)

func _on_dialogic_text_signal(argument:String):
    if argument == "activate_something":
        print("Something was activated!")
```

---

## 3. Start & End signals

Using the `Dialogic.timeline_ended` and `Dialogic.timeline_started` signals (both have no arguments) lets you react to dialog ending or beginning.

Example:

```gdscript
func start_dialog():
    Dialogic.timeline_ended.connect(_on_timeline_ended)
    Dialogic.start("my_timeline")

func _on_timeline_ended():
    Dialogic.timeline_ended.disconnect(_on_timeline_ended)
    # do something else here
```

---

## 4. Subsystem signals

Dialogic subsystems have many useful signals. Here is a selection of them:

- `Dialogic.Text` has

    - signal `about_to_show_text(info:Dictionary)`
    - signal `text_finished(info:Dictionary)`
    - signal `speaker_updated(character:DialogicCharacter)`
    - signal `textbox_visibility_changed(visible:bool)`
    - signal `animation_textbox_new_text`
    - signal `animation_textbox_show`
    - signal `animation_textbox_hide`

- `Dialogic.Portraits` has

    - signal `character_joined(info:Dictionary)`
    - signal `character_left(info:Dictionary)`
    - signal `character_portrait_changed(info:Dictionary)`

- `Dialogic.VAR` has

    - signal `variable_changed(info:Dictionary)`
    - signal `variable_was_set(info:Dictionary)` # only on set variable events

If you want to find all signals, head over to the [Subsystem Index](subsystem_class_index.md), select a subsystem and take a look at the related **Signals** category.
