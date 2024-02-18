
<div class="header-banner purple">
<div class="header-label purple">DialogicGameHandler</div>
</div>

*This contains the source code documentation of the class `DialogicGameHandler`.*
        
# DialogicGameHandler
**Inherits:** Node

Autoload script that allows interacting with all of Dialogics systems: - Holds all important information about the current state of Dialogic. - Gives access to all the subystems. - Has methods to start timelines.
## Properties
Name | Type | Default 
--- | --- | --- 
Animations | `Modules/Core/subsystem_animation.gd` |   
Audio | `Modules/Audio/subsystem_audio.gd` |   
Backgrounds | `Modules/Background/subsystem_backgrounds.gd` |   
Choices | `Modules/Choice/subsystem_choices.gd` |   
Expressions | `Modules/Core/subsystem_expression.gd` |   
Glossary | `Modules/Glossary/subsystem_glossary.gd` |   
History | `Modules/History/subsystem_history.gd` |   
Inputs | `Modules/Core/subsystem_input.gd` |   
Jump | `Modules/Jump/subsystem_jump.gd` |   
Portraits | `Modules/Character/subsystem_portraits.gd` |   
Save | `Modules/Save/subsystem_save.gd` |   
Settings | `Modules/Settings/subsystem_settings.gd` |   
Styles | `Modules/Style/subsystem_styles.gd` |   
Text | `Modules/Text/subsystem_text.gd` |   
TextInput | `Modules/TextInput/subsystem_text_input.gd` |   
VAR | `Modules/Variable/subsystem_variables.gd` |   
Voice | `Modules/Voice/subsystem_voice.gd` |   
current_event_idx | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
current_state | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
current_state_info | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
current_timeline | [DialogicTimeline](class_dialogictimeline.md) |  `null` 
current_timeline_events | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |   
paused | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_subsystem</span>](#property-add_subsystem) ( `_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `_script_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">clear</span>](#property-clear) ( `clear_flags`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">collect_subsystems</span>](#property-collect_subsystems) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">end_timeline</span>](#property-end_timeline) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_full_state</span>](#property-get_full_state) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_subsystem</span>](#property-get_subsystem) ( `_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">handle_event</span>](#property-handle_event) ( `event_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">handle_next_event</span>](#property-handle_next_event) ( `ignore_argument`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">has_subsystem</span>](#property-has_subsystem) ( `_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">load_full_state</span>](#property-load_full_state) ( `state_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">preload_timeline</span>](#property-preload_timeline) ( `timeline_resource`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">start</span>](#property-start) ( `timeline`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `label`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">start_timeline</span>](#property-start_timeline) ( `timeline`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `label_or_idx`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` ) 
--- 
## Constants


<a class="header" id="constant-IDLE" href="#constant-IDLE">**<span class="hljs-attribute">const</span> <span class="hljs-title">IDLE</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-REVEALING_TEXT" href="#constant-REVEALING_TEXT">**<span class="hljs-attribute">const</span> <span class="hljs-title">REVEALING_TEXT</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ANIMATING" href="#constant-ANIMATING">**<span class="hljs-attribute">const</span> <span class="hljs-title">ANIMATING</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-AWAITING_CHOICE" href="#constant-AWAITING_CHOICE">**<span class="hljs-attribute">const</span> <span class="hljs-title">AWAITING_CHOICE</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-WAITING" href="#constant-WAITING">**<span class="hljs-attribute">const</span> <span class="hljs-title">WAITING</span><span class="hljs-comment"> = 4</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-FULL_CLEAR" href="#constant-FULL_CLEAR">**<span class="hljs-attribute">const</span> <span class="hljs-title">FULL_CLEAR</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-KEEP_VARIABLES" href="#constant-KEEP_VARIABLES">**<span class="hljs-attribute">const</span> <span class="hljs-title">KEEP_VARIABLES</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TIMLEINE_INFO_ONLY" href="#constant-TIMLEINE_INFO_ONLY">**<span class="hljs-attribute">const</span> <span class="hljs-title">TIMLEINE_INFO_ONLY</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-dialogic_paused" href="#signal-dialogic_paused">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">dialogic_paused</span>](#signal-dialogic_paused) ( )** </a>



Emitted when [paused] changes to true.

---



<a class="header" id="signal-dialogic_resumed" href="#signal-dialogic_resumed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">dialogic_resumed</span>](#signal-dialogic_resumed) ( )** </a>



Emitted when [paused] changes to false.

---



<a class="header" id="signal-event_handled" href="#signal-event_handled">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">event_handled</span>](#signal-event_handled) ( `resource`: [DialogicEvent](class_dialogicevent.md) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-signal_event" href="#signal-signal_event">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">signal_event</span>](#signal-signal_event) ( `argument`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



Emitted when the Signal event was reached

---



<a class="header" id="signal-state_changed" href="#signal-state_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">state_changed</span>](#signal-state_changed) ( `new_state`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )** </a>



Emitted when [current_state] change.

---



<a class="header" id="signal-text_signal" href="#signal-text_signal">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">text_signal</span>](#signal-text_signal) ( `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



Emitted when [signal] effect was reached in text.

---



<a class="header" id="signal-timeline_ended" href="#signal-timeline_ended">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">timeline_ended</span>](#signal-timeline_ended) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-timeline_started" href="#signal-timeline_started">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">timeline_started</span>](#signal-timeline_started) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-add_subsystem" href="#property-add_subsystem">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_subsystem</span>](#property-add_subsystem) ( `_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `_script_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-clear" href="#property-clear">**<span class="hljs-attribute">void</span> [<span class="hljs-title">clear</span>](#property-clear) ( `clear_flags`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )** </a>



Resets dialogics state fully or partially. By using the clear flags you can specify what info should be kept. For example at timeline end usually it doesn't clear node or subsystem info

---



<a class="header" id="property-collect_subsystems" href="#property-collect_subsystems">**<span class="hljs-attribute">void</span> [<span class="hljs-title">collect_subsystems</span>](#property-collect_subsystems) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-end_timeline" href="#property-end_timeline">**<span class="hljs-attribute">void</span> [<span class="hljs-title">end_timeline</span>](#property-end_timeline) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_full_state" href="#property-get_full_state">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_full_state</span>](#property-get_full_state) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_subsystem" href="#property-get_subsystem">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_subsystem</span>](#property-get_subsystem) ( `_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-handle_event" href="#property-handle_event">**<span class="hljs-attribute">void</span> [<span class="hljs-title">handle_event</span>](#property-handle_event) ( `event_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-handle_next_event" href="#property-handle_next_event">**<span class="hljs-attribute">void</span> [<span class="hljs-title">handle_next_event</span>](#property-handle_next_event) ( `ignore_argument`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-has_subsystem" href="#property-has_subsystem">**<span class="hljs-attribute">void</span> [<span class="hljs-title">has_subsystem</span>](#property-has_subsystem) ( `_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-load_full_state" href="#property-load_full_state">**<span class="hljs-attribute">void</span> [<span class="hljs-title">load_full_state</span>](#property-load_full_state) ( `state_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-preload_timeline" href="#property-preload_timeline">**<span class="hljs-attribute">void</span> [<span class="hljs-title">preload_timeline</span>](#property-preload_timeline) ( `timeline_resource`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-start" href="#property-start">**<span class="hljs-attribute">void</span> [<span class="hljs-title">start</span>](#property-start) ( `timeline`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `label`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` )** </a>



Method to start a timeline AND ensure that a layout scene is present. For argument info, checkout start_timeline() -> returns the layout node

---



<a class="header" id="property-start_timeline" href="#property-start_timeline">**<span class="hljs-attribute">void</span> [<span class="hljs-title">start_timeline</span>](#property-start_timeline) ( `timeline`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `label_or_idx`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` )** </a>



Method to start a timeline without adding a layout scene. @timeline can be either a loaded timeline resource or a path to a timeline file. @label_or_idx can be a label (string) or index (int) to skip to immediatly.

---

