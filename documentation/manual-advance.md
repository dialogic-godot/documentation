<div class="header-banner purple">
     <div class="header-label purple">Manual-Advance</div>
</div>

*Manual-Advance allows your player to advance the timeline by using input mapped to `dialogic_default_action` (Project Settings → Input Map).*

## 📜 Content
[toc]

## 1. What is Manual-Advance?

Manual-Advance is a feature in Dialogic that allows players to progress through the timeline *with* inputs! It's enabled by default: The player clicks, and the timeline moves down its stack of events.

## 2. Changing Manual-Advance via Code

Dialogic's Manual-Advance class can be easily accessed via the Inputs subsystem and allows you to change Manual-Advance during your game. It also has a number of settings not exposed to the dialogic interface.

All of this functionality lives in `Dialogic.Inputs.Manual-Advance` an `DialogicManualAdvance` object.
We can limit the player from interacting with the timeline to display a scripted timeline section.

### 2.1 Limit Player Inputs via Code
It's straightforward to script this behaviour. The following snippet showcases this:

```gdscript
Dialogic.Inputs.auto_advance.disabled_until_next_event = true
```

In Dialogic, both Manual-Advance and Auto-Advance share the concept of `system`: The system is the feature itself, in this case Manual-Advance. You can prevent players from advancing the timeline:

```gdscript
# No more inputs for you, player.
Dialogic.Inputs.auto_advance.system_enabled = false
```

Additionally, you can call the method `Dialogic.Inputs.auto_advance.is_enabled()` to check if the player can manually advance.
