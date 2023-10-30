---
title: Auto-Skip
---

![header_getting_started](/media/headers/autoadvance.png)

## What is Auto-Skip?
Auto-Skip is the concept of advancing a timeline until an unseen text or
an interactive event is reached.

In Visual Novels, Auto-Skip helps to navigate already known story branches quickly.
If your story is not intended to be cyclic, this feature may not be of use to you.

There are two types of this feature:

- Timed Auto-Skip, moving through the timeline by a set maximum delay per event.
- Instant Auto-Skip, finding the next valid point within one frame.

Some Visual Novels offer one or both flavours of Auto-Skip.

> **Note:** \
*Instant* Auto-Skip has not been implemented yet.

## How to use it?

In Dialogic, Auto-Skip can be controlled via the scripting API. If you want to provide the player with an Auto-Skip toggle button, this section will teach you how to implement the logic.

First, you can set the time each event is allowed to take via the Text settings page inside Dialogic.

![header_saving_loading](/media/auto-skip/auto_skip_settings.png)

However, there are many settings hiding inside the scripting API!

## Scripting Auto-Skip

All settings reside as variables on the `AutoSkip` class located at `Dialogic.Text.auto_skip`. Hence, you can set the variables to your heart's content!

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

Aforementioned, this is code snippet is useful for debugging.\
Don't forget to set `Dialogic.Text.auto_skip.disable_on_unread_text` back to `true` again, if you want to test the normal skipping behaviour.


For more information, check the scripting documentation!\
Each variable contains useful descriptions and displays the default values.

## Custom Events

Events come in all sort of behaviours: Delaying input, conditionally branching, fading images, playing audio, …

It's impossible to let an Auto-Skip handle all of these effects gracefully from the outside.

Therefore, Auto-Skip’s behaviour is implemented by each Timeline Event. Every event can check if Auto-Skip is enabled via `Dialogic.Text.auto_skip.enabled` and then check the time an event may take via `Dialogic.Text.auto_skip.time_per_event`.