---
title: Auto-Skip
---

![header_getting_started](/media/headers/autoadvance.png)

## What is Auto-Skip?
Auto-Skip is the concept of advancing a timeline faster than you can read it.

In Visual Novels, Auto-Skip helps to navigate already known story branches quickly.
If your story is not intended to be cyclic, this feature may not be of use to you.


> **Note:** \
*Instant* Auto-Skip has not been implemented yet.

## How to use it?

In Dialogic, Auto-Skip can be controlled via the scripting API. If you want to provide the player with an Auto-Skip toggle button, this section will teach you how to implement the logic.

First, you can set the time each event is allowed to take via the Text settings page inside Dialogic.

![header_saving_loading](/media/auto-skip/auto_skip_settings.png)

However, there are many settings hiding inside the scripting API!

## Scripting Auto-Skip

All Auto-Skip settings are variables on the `AutoSkip` class.
This class can be accessed via `Dialogic.Text.auto_skip`.

First, imagine you want to add an Auto-Skip button to your game. You can use the following code to toggle the feature on and off:

```gdscript
Dialogic.Text.auto_skip.enabled = !Dialogic.Text.auto_skip.enabled
```

Furthermore, think about quickly debugging your timeline, you can use *Jump* and *Label Events* for this, or create your own Auto-Skip debug mode.\
The upcoming code can help you toggle this behaviour:

```gdscript
Dialogic.Text.auto_skip.enabled = !Dialogic.Text.auto_skip.enabled

# We can slow the Auto-Skip down to have better control stopping it.
Dialogic.Text.auto_skip.time_per_event = 0.3

# Important!
# By default, Auto-Skip cancels on unread text.
Dialogic.Text.auto_skip.disable_on_unread_text = false
```
Don't forget to set `disable_on_unread_text` back to `true` again, if you want to return to the default behaviour again.

For more information, check the scripting documentation on the `AutoSkip` class!\
Each variable contains useful descriptions and displays the default values.

## Signals
When Auto-Skip is enabled or disabled, the feature will emit `signal autoskip_changed(is_enabled: bool)`.

As an example, internally, Dialogic uses this signal to handle skipping for *Text Events* when the event is revealing text or waiting for the user to manually advance.

```gdscript
# This method has been connected to the autoskip_changed signal.
func _on_autoskip_enable(enabled: bool):
	if not enabled:
		return

	if state == States.REVEALING:
		Dialogic.Text.skip_text_animation()

	advance.emit()
```

## Custom Events

Events come in all sort of behaviours: Awaiting signals, instantly executing, a mix of conditions, playing audio, …\
It's impossible to let an Auto-Skip handle all of these effects gracefully from the outside.\
Therefore, Auto-Skip's behaviour must be implemented by each Timeline Event.

### What type of event do I have?
Does your event finish instantly? Does it play audio? Does it await a signal?\
These situations must be implemented differently.

If you await signals, you can use the `autoskip_changed` signal to cause your event to react to Auto-Skip.\
The Text Event uses this signal to skip the text animation and then advance the timeline.

If you await a timer or perform an action lasting multiple frames, you can use the `time_per_event` variable to limit the time your event may take.\
Here is a code snippet to give you an idea:
```gdscript
var animation_length: float = 10.0

if Dialogic.Text.auto_skip.enabled:
    var time_per_event: float = Dialogic.Text.auto_skip.time_per_event
    animation_length = min(time_per_event, animation_length)
```

This code will cap the animation length to the maximum time set, if Auto-Skip is enabled.