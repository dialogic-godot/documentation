
<div class="header-banner purple">
<div class="header-label purple">Input</div>
</div>

*This contains the source code documentation of the class `subsystem_Input`.*
        
# subsystem_Input
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that handles input, Auto-Advance, and skipping.
## Description
This subsystem can be accessed via GDScript: `Dialogic.Inputs`.

## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">input_block_timer</span>](#property-input_block_timer) | [Timer](https://docs.godotengine.org/en/latest/classes/class_timer.html#class-timer) |  `new()` 
[<span class="hljs-title">action_was_consumed</span>](#property-action_was_consumed) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">auto_skip</span>](#property-auto_skip) | [DialogicAutoSkip](class_dialogicautoskip.md) |  `null` 
[<span class="hljs-title">auto_advance</span>](#property-auto_advance) | [DialogicAutoAdvance](class_dialogicautoadvance.md) |  `null` 
[<span class="hljs-title">manual_advance</span>](#property-manual_advance) | [DialogicManualAdvance](class_dialogicmanualadvance.md) |  `null` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">pause</span>](#method-pause) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume</span>](#method-resume) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">post_install</span>](#method-post_install) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">handle_input</span>](#method-handle_input) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_input_pressed</span>](#method-is_input_pressed) ( `event`: [InputEvent](https://docs.godotengine.org/en/latest/classes/class_inputevent.html#class-inputevent), `exact`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">handle_node_gui_input</span>](#method-handle_node_gui_input) ( `event`: [InputEvent](https://docs.godotengine.org/en/latest/classes/class_inputevent.html#class-inputevent) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_input_blocked</span>](#method-is_input_blocked) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">block_input</span>](#method-block_input) ( `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.1` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">stop_timers</span>](#method-stop_timers) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">start_autoskip_timer</span>](#method-start_autoskip_timer) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_input</span>](#method-effect_input) ( `_text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `_argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_noskip</span>](#method-effect_noskip) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_autoadvance</span>](#method-effect_autoadvance) ( `_text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `_skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
--- 

## Signals


<a class="header" id="signal-dialogic_action_priority" href="#signal-dialogic_action_priority">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">dialogic_action_priority</span>](#signal-dialogic_action_priority) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-dialogic_action" href="#signal-dialogic_action">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">dialogic_action</span>](#signal-dialogic_action) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-autoskip_timer_finished" href="#signal-autoskip_timer_finished">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">autoskip_timer_finished</span>](#signal-autoskip_timer_finished) ( )** </a>



 Whenever the Auto-Skip timer finishes, this signal is emitted. Configure Auto-Skip settings via `auto_skip`. 

---

## Property Descriptions



<a class="header" id="property-input_block_timer" href="#property-input_block_timer">**<span class="hljs-attribute">var</span> <span class="hljs-title">input_block_timer</span> <span style = "color: gray"> = </span> new()** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-action_was_consumed" href="#property-action_was_consumed">**<span class="hljs-attribute">var</span> <span class="hljs-title">action_was_consumed</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-auto_skip" href="#property-auto_skip">**<span class="hljs-attribute">var</span> <span class="hljs-title">auto_skip</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-auto_advance" href="#property-auto_advance">**<span class="hljs-attribute">var</span> <span class="hljs-title">auto_advance</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-manual_advance" href="#property-manual_advance">**<span class="hljs-attribute">var</span> <span class="hljs-title">manual_advance</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-pause" href="#method-pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pause</span>](#method-pause) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-resume" href="#method-resume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume</span>](#method-resume) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-post_install" href="#method-post_install">**<span class="hljs-attribute">func</span> [<span class="hljs-title">post_install</span>](#method-post_install) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-handle_input" href="#method-handle_input">**<span class="hljs-attribute">func</span> [<span class="hljs-title">handle_input</span>](#method-handle_input) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_input_pressed" href="#method-is_input_pressed">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_input_pressed</span>](#method-is_input_pressed) ( `event`: [InputEvent](https://docs.godotengine.org/en/latest/classes/class_inputevent.html#class-inputevent), `exact`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-handle_node_gui_input" href="#method-handle_node_gui_input">**<span class="hljs-attribute">func</span> [<span class="hljs-title">handle_node_gui_input</span>](#method-handle_node_gui_input) ( `event`: [InputEvent](https://docs.godotengine.org/en/latest/classes/class_inputevent.html#class-inputevent) )</a>  ⇒ <span style = "color: gray">void</span>** 



This is called from the gui_input of the InputCatcher and DialogText nodes

---



<a class="header" id="method-is_input_blocked" href="#method-is_input_blocked">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_input_blocked</span>](#method-is_input_blocked) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-block_input" href="#method-block_input">**<span class="hljs-attribute">func</span> [<span class="hljs-title">block_input</span>](#method-block_input) ( `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.1` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-stop_timers" href="#method-stop_timers">**<span class="hljs-attribute">func</span> [<span class="hljs-title">stop_timers</span>](#method-stop_timers) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-start_autoskip_timer" href="#method-start_autoskip_timer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">start_autoskip_timer</span>](#method-start_autoskip_timer) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



This method will advance the timeline based on Auto-Skip settings. The state, whether Auto-Skip is enabled, is ignored.

---



<a class="header" id="method-effect_input" href="#method-effect_input">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_input</span>](#method-effect_input) ( `_text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `_argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-effect_noskip" href="#method-effect_noskip">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_noskip</span>](#method-effect_noskip) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-effect_autoadvance" href="#method-effect_autoadvance">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_autoadvance</span>](#method-effect_autoadvance) ( `_text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `_skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

