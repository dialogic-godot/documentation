
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
[<span class="hljs-title">autoadvance_timer</span>](#property-autoadvance_timer) | [Timer](https://docs.godotengine.org/en/latest/classes/class_timer.html#class-timer) |   
[<span class="hljs-title">await_playing_voice</span>](#property-await_playing_voice) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">delay_modifier</span>](#property-delay_modifier) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `1.0` 
[<span class="hljs-title">enabled_forced</span>](#property-enabled_forced) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">enabled_until_next_event</span>](#property-enabled_until_next_event) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">enabled_until_user_input</span>](#property-enabled_until_user_input) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">fixed_delay</span>](#property-fixed_delay) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `1.0` 
[<span class="hljs-title">ignored_characters</span>](#property-ignored_characters) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">ignored_characters_enabled</span>](#property-ignored_characters_enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">override_delay_for_current_event</span>](#property-override_delay_for_current_event) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `-1.0` 
[<span class="hljs-title">per_character_delay</span>](#property-per_character_delay) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.1` 
[<span class="hljs-title">per_word_delay</span>](#property-per_word_delay) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span> | [<span class="hljs-title">get_progress</span>](#method-get_progress) ( ) 
<span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span> | [<span class="hljs-title">get_time</span>](#method-get_time) ( ) 
<span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span> | [<span class="hljs-title">get_time_left</span>](#method-get_time_left) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_advancing</span>](#method-is_advancing) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_enabled</span>](#method-is_enabled) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">start</span>](#method-start) ( ) 
--- 

## Signals


<a class="header" id="signal-autoadvance" href="#signal-autoadvance">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">autoadvance</span>](#signal-autoadvance) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-toggled" href="#signal-toggled">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">toggled</span>](#signal-toggled) ( `enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-autoadvance_timer" href="#property-autoadvance_timer">**<span class="hljs-attribute">var</span> <span class="hljs-title">autoadvance_timer</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-await_playing_voice" href="#property-await_playing_voice">**<span class="hljs-attribute">var</span> <span class="hljs-title">await_playing_voice</span> <span style = "color: gray"> = </span> true** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-delay_modifier" href="#property-delay_modifier">**<span class="hljs-attribute">var</span> <span class="hljs-title">delay_modifier</span> <span style = "color: gray"> = </span> 1.0** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-enabled_forced" href="#property-enabled_forced">**<span class="hljs-attribute">var</span> <span class="hljs-title">enabled_forced</span> <span style = "color: gray"> = </span> false** 



If true, Auto-Advance will stay enabled until this is set to false.  This boolean can be used to create an automatic text display.  Stacks with `enabled_until_next_event` and `enabled_until_user_input`.

---



<a class="header" id="property-enabled_until_next_event" href="#property-enabled_until_next_event">**<span class="hljs-attribute">var</span> <span class="hljs-title">enabled_until_next_event</span> <span style = "color: gray"> = </span> false** 



If true, Auto-Advance will be active until the next event.  Use this flag to create a temporary Auto-Advance mode. You can utilise `override_delay_for_current_event` to set a temporary Auto-Advance delay for this event.  Stacks with `enabled_forced` and `enabled_until_user_input`.

---



<a class="header" id="property-enabled_until_user_input" href="#property-enabled_until_user_input">**<span class="hljs-attribute">var</span> <span class="hljs-title">enabled_until_user_input</span> <span style = "color: gray"> = </span> false** 



If true, Auto-Advance will be active until the player presses a button.  Use this flag when the player wants to enable Auto-Advance.  Stacks with `enabled_forced` and `enabled_until_next_event`.

---



<a class="header" id="property-fixed_delay" href="#property-fixed_delay">**<span class="hljs-attribute">var</span> <span class="hljs-title">fixed_delay</span> <span style = "color: gray"> = </span> 1.0** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-ignored_characters" href="#property-ignored_characters">**<span class="hljs-attribute">var</span> <span class="hljs-title">ignored_characters</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-ignored_characters_enabled" href="#property-ignored_characters_enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">ignored_characters_enabled</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-override_delay_for_current_event" href="#property-override_delay_for_current_event">**<span class="hljs-attribute">var</span> <span class="hljs-title">override_delay_for_current_event</span> <span style = "color: gray"> = </span> -1.0** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-per_character_delay" href="#property-per_character_delay">**<span class="hljs-attribute">var</span> <span class="hljs-title">per_character_delay</span> <span style = "color: gray"> = </span> 0.1** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-per_word_delay" href="#property-per_word_delay">**<span class="hljs-attribute">var</span> <span class="hljs-title">per_word_delay</span> <span style = "color: gray"> = </span> 0.0** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-get_progress" href="#method-get_progress">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_progress</span>](#method-get_progress) ( )</a>  ⇒ <span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span>** 



Returns the progress of the auto-advance timer on a scale between 0 and 1. The higher the value, the closer the timer is to finishing. If auto-advancing is disabled, returns -1.

---



<a class="header" id="method-get_time" href="#method-get_time">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_time</span>](#method-get_time) ( )</a>  ⇒ <span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_time_left" href="#method-get_time_left">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_time_left</span>](#method-get_time_left) ( )</a>  ⇒ <span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_advancing" href="#method-is_advancing">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_advancing</span>](#method-is_advancing) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_enabled" href="#method-is_enabled">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_enabled</span>](#method-is_enabled) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns whether Auto-Advance is currently considered enabled. Auto-Advance uses three different enable flags: - enabled_until_user_input (becomes false on any dialogic input action) - enabled_until_next_event (becomes false on each text event) - enabled_forced (becomes false only when disabled via code)  All three can be set with dedicated methods.

---



<a class="header" id="method-start" href="#method-start">**<span class="hljs-attribute">func</span> [<span class="hljs-title">start</span>](#method-start) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

