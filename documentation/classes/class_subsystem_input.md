
<div class="header-banner purple">
<div class="header-label purple">subsystem_input</div>
</div>

*This contains the source code documentation of the class `subsystem_input`.*
        
# subsystem_input
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

##############################################################################
## Properties
Name | Type | Default 
--- | --- | --- 
action_was_consumed | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
auto_advance | [DialogicAutoAdvance](class_dialogicautoadvance.md) |  `null` 
auto_skip | [DialogicAutoSkip](class_dialogicautoskip.md) |  `null` 
input_block_timer | [Timer](https://docs.godotengine.org/en/latest/classes/class_timer.html#class-timer) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">block_input</span>](#property-block_input) ( `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.1` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_autoadvance</span>](#property-effect_autoadvance) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_input</span>](#property-effect_input) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_noskip</span>](#property-effect_noskip) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">handle_input</span>](#property-handle_input) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_input_blocked</span>](#property-is_input_blocked) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_manualadvance_enabled</span>](#property-is_manualadvance_enabled) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">pause</span>](#property-pause) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">post_install</span>](#property-post_install) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume</span>](#property-resume) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_manualadvance</span>](#property-set_manualadvance) ( `enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `temp`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">start_autoskip_timer</span>](#property-start_autoskip_timer) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">stop_timers</span>](#property-stop_timers) ( ) 
--- 

## Signals


<a class="header" id="signal-autoskip_timer_finished" href="#signal-autoskip_timer_finished">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">autoskip_timer_finished</span>](#signal-autoskip_timer_finished) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-dialogic_action" href="#signal-dialogic_action">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">dialogic_action</span>](#signal-dialogic_action) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-dialogic_action_priority" href="#signal-dialogic_action_priority">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">dialogic_action_priority</span>](#signal-dialogic_action_priority) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-block_input" href="#property-block_input">**<span class="hljs-attribute">func</span> [<span class="hljs-title">block_input</span>](#property-block_input) ( `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.1` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-clear_game_state" href="#property-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-effect_autoadvance" href="#property-effect_autoadvance">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_autoadvance</span>](#property-effect_autoadvance) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-effect_input" href="#property-effect_input">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_input</span>](#property-effect_input) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-effect_noskip" href="#property-effect_noskip">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_noskip</span>](#property-effect_noskip) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-handle_input" href="#property-handle_input">**<span class="hljs-attribute">func</span> [<span class="hljs-title">handle_input</span>](#property-handle_input) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_input_blocked" href="#property-is_input_blocked">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_input_blocked</span>](#property-is_input_blocked) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_manualadvance_enabled" href="#property-is_manualadvance_enabled">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_manualadvance_enabled</span>](#property-is_manualadvance_enabled) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-pause" href="#property-pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pause</span>](#property-pause) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-post_install" href="#property-post_install">**<span class="hljs-attribute">func</span> [<span class="hljs-title">post_install</span>](#property-post_install) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-resume" href="#property-resume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume</span>](#property-resume) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_manualadvance" href="#property-set_manualadvance">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_manualadvance</span>](#property-set_manualadvance) ( `enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `temp`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-start_autoskip_timer" href="#property-start_autoskip_timer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">start_autoskip_timer</span>](#property-start_autoskip_timer) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



This method will advance the timeline based on Auto-Skip settings. The state, whether Auto-Skip is enabled, is ignored.

---



<a class="header" id="property-stop_timers" href="#property-stop_timers">**<span class="hljs-attribute">func</span> [<span class="hljs-title">stop_timers</span>](#property-stop_timers) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

