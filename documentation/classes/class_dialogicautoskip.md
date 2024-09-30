
<div class="header-banner purple">
<div class="header-label purple">DialogicAutoSkip</div>
</div>

*This contains the source code documentation of the class `DialogicAutoSkip`.*
        
# DialogicAutoSkip
**Inherits:** [RefCounted](https://docs.godotengine.org/en/latest/classes/class_refcounted.html#class-refcounted)

This class holds the settings for the Auto-Skip feature. Changing the variables will alter the behaviour of Auto-Skip.
## Description
Auto-Skip must be implemented per event.

## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">enabled</span>](#property-enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">disable_on_user_input</span>](#property-disable_on_user_input) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">disable_on_unread_text</span>](#property-disable_on_unread_text) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">enable_on_visited</span>](#property-enable_on_visited) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">skip_voice</span>](#property-skip_voice) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">time_per_event</span>](#property-time_per_event) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.1` 

## Signals


<a class="header" id="signal-toggled" href="#signal-toggled">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">toggled</span>](#signal-toggled) ( `is_enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) )** </a>



 Emitted whenever the Auto-Skip state changes, from `true` to `false` or vice-versa. 

---

## Property Descriptions



<a class="header" id="property-enabled" href="#property-enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">enabled</span> <span style = "color: gray"> = </span> false** 



Whether Auto-Skip is enabled or not. If Auto-Skip is referred to be disabled[/i], it refers to setting this this variable to `false`. This variable will automatically emit [autoskip_changed](#signal-autoskip_changed) when changed.

---



<a class="header" id="property-disable_on_user_input" href="#property-disable_on_user_input">**<span class="hljs-attribute">var</span> <span class="hljs-title">disable_on_user_input</span> <span style = "color: gray"> = </span> true** 



If `true`, Auto-Skip will be disabled when the user presses a recognised input action.

---



<a class="header" id="property-disable_on_unread_text" href="#property-disable_on_unread_text">**<span class="hljs-attribute">var</span> <span class="hljs-title">disable_on_unread_text</span> <span style = "color: gray"> = </span> false** 



If `true`, Auto-Skip will be disabled when the timeline advances to a unread Text event or an event requesting user input.

---



<a class="header" id="property-enable_on_visited" href="#property-enable_on_visited">**<span class="hljs-attribute">var</span> <span class="hljs-title">enable_on_visited</span> <span style = "color: gray"> = </span> false** 



If `true`, Auto-Skip will be enabled when the timeline advances to a previously visited Text event. Useful if the player always wants to skip already-visited Text events.

---



<a class="header" id="property-skip_voice" href="#property-skip_voice">**<span class="hljs-attribute">var</span> <span class="hljs-title">skip_voice</span> <span style = "color: gray"> = </span> true** 



If `true`, Auto-Skip will skip Voice events instead of playing them.

---



<a class="header" id="property-time_per_event" href="#property-time_per_event">**<span class="hljs-attribute">var</span> <span class="hljs-title">time_per_event</span> <span style = "color: gray"> = </span> 0.1** 



The amount of seconds each event may take. This is not enforced, each event must implement this behaviour.

---

