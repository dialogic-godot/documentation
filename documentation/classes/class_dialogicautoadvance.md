
<div class="header-banner purple">
<div class="header-label purple">DialogicAutoAdvance</div>
</div>

*This contains the source code documentation of the class `DialogicAutoAdvance`.*
        
# DialogicAutoAdvance
**Inherits:** [RefCounted](https://docs.godotengine.org/en/latest/classes/class_refcounted.html#class-refcounted)

This class holds the settings for the Auto-Advance feature. Changing the variables will alter the behaviour of Auto-Advance.
## Description
Auto-Advance is a feature that automatically advances the timeline after a player-specific amount of time. This is useful for visual novels that want the player to read the text without having to press.  Unlike [DialogicAutoSkip](class_dialogicautoskip.md), Auto-Advance uses multiple enable flags, allowing to track the different instances that enabled Auto-Advance. For instance, if a timeline event forces Auto-Advance to be enabled and later disables it, the Auto-Advance will still be enabled if the player didn't cancel it.

## Properties
Name | Type | Default 
--- | --- | --- 
autoadvance_timer | [Timer](https://docs.godotengine.org/en/latest/classes/class_timer.html#class-timer) |   
await_playing_voice | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
delay_modifier | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `1.0` 
enabled_forced | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
enabled_until_next_event | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
enabled_until_user_input | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
fixed_delay | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `1.0` 
ignored_characters | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
ignored_characters_enabled | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
override_delay_for_current_event | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `-1.0` 
per_character_delay | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.1` 
per_word_delay | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_progress</span>](#property-get_progress) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_time</span>](#property-get_time) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_time_left</span>](#property-get_time_left) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">is_advancing</span>](#property-is_advancing) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">is_enabled</span>](#property-is_enabled) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">start</span>](#property-start) ( ) 
--- 

## Signals


<a class="header" id="signal-autoadvance" href="#signal-autoadvance">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">autoadvance</span>](#signal-autoadvance) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-toggled" href="#signal-toggled">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">toggled</span>](#signal-toggled) ( `enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-get_progress" href="#property-get_progress">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_progress</span>](#property-get_progress) ( )** </a>



Returns the progress of the auto-advance timer on a scale between 0 and 1. The higher the value, the closer the timer is to finishing. If auto-advancing is disabled, returns -1.

---



<a class="header" id="property-get_time" href="#property-get_time">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_time</span>](#property-get_time) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_time_left" href="#property-get_time_left">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_time_left</span>](#property-get_time_left) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_advancing" href="#property-is_advancing">**<span class="hljs-attribute">void</span> [<span class="hljs-title">is_advancing</span>](#property-is_advancing) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_enabled" href="#property-is_enabled">**<span class="hljs-attribute">void</span> [<span class="hljs-title">is_enabled</span>](#property-is_enabled) ( )** </a>



Returns whether Auto-Advance is currently considered enabled. Auto-Advance uses three different enable flags: - enabled_until_user_input (becomes false on any dialogic input action) - enabled_until_next_event (becomes false on each text event) - enabled_forced (becomes false only when disabled via code)  All three can be set with dedicated methods.

---



<a class="header" id="property-start" href="#property-start">**<span class="hljs-attribute">void</span> [<span class="hljs-title">start</span>](#property-start) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

