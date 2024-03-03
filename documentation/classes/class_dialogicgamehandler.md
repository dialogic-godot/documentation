
<div class="header-banner purple">
<div class="header-label purple">DialogicGameHandler</div>
</div>

*This contains the source code documentation of the class `DialogicGameHandler`.*
        
# DialogicGameHandler
**Inherits:** [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)

Autoload script that allows you to interact with all of Dialogic's systems:
- Holds all important information about the current state of Dialogic.
- Provides access to all the subsystems.
- Has methods to start/end timelines.

## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">Animations</span>](#property-animations) | `Modules/Core/subsystem_animation.gd` |   
[<span class="hljs-title">Audio</span>](#property-audio) | `Modules/Audio/subsystem_audio.gd` |   
[<span class="hljs-title">Backgrounds</span>](#property-backgrounds) | `Modules/Background/subsystem_backgrounds.gd` |   
[<span class="hljs-title">Choices</span>](#property-choices) | `Modules/Choice/subsystem_choices.gd` |   
[<span class="hljs-title">Expressions</span>](#property-expressions) | `Modules/Core/subsystem_expression.gd` |   
[<span class="hljs-title">Glossary</span>](#property-glossary) | `Modules/Glossary/subsystem_glossary.gd` |   
[<span class="hljs-title">History</span>](#property-history) | `Modules/History/subsystem_history.gd` |   
[<span class="hljs-title">Inputs</span>](#property-inputs) | `Modules/Core/subsystem_input.gd` |   
[<span class="hljs-title">Jump</span>](#property-jump) | `Modules/Jump/subsystem_jump.gd` |   
[<span class="hljs-title">Portraits</span>](#property-portraits) | `Modules/Character/subsystem_portraits.gd` |   
[<span class="hljs-title">Save</span>](#property-save) | `Modules/Save/subsystem_save.gd` |   
[<span class="hljs-title">Settings</span>](#property-settings) | `Modules/Settings/subsystem_settings.gd` |   
[<span class="hljs-title">Styles</span>](#property-styles) | `Modules/Style/subsystem_styles.gd` |   
[<span class="hljs-title">Text</span>](#property-text) | `Modules/Text/subsystem_text.gd` |   
[<span class="hljs-title">TextInput</span>](#property-textinput) | `Modules/TextInput/subsystem_text_input.gd` |   
[<span class="hljs-title">VAR</span>](#property-var) | `Modules/Variable/subsystem_variables.gd` |   
[<span class="hljs-title">Voice</span>](#property-voice) | `Modules/Voice/subsystem_voice.gd` |   
[<span class="hljs-title">current_event_idx</span>](#property-current_event_idx) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">current_state</span>](#property-current_state) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">current_state_info</span>](#property-current_state_info) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">current_timeline</span>](#property-current_timeline) | [DialogicTimeline](class_dialogictimeline.md) |  `null` 
[<span class="hljs-title">current_timeline_events</span>](#property-current_timeline_events) | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |   
[<span class="hljs-title">paused</span>](#property-paused) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[DialogicSubsystem](class_dialogicsubsystem.md)</span> | [<span class="hljs-title">add_subsystem</span>](#method-add_subsystem) ( `subsystem_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `script_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">clear</span>](#method-clear) ( `clear_flags`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">end_timeline</span>](#method-end_timeline) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_full_state</span>](#method-get_full_state) ( ) 
<span class="hljs-attribute">[DialogicSubsystem](class_dialogicsubsystem.md)</span> | [<span class="hljs-title">get_subsystem</span>](#method-get_subsystem) ( `subsystem_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">handle_event</span>](#method-handle_event) ( `event_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">handle_next_event</span>](#method-handle_next_event) ( `ignore_argument`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_subsystem</span>](#method-has_subsystem) ( `subsystem_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_full_state</span>](#method-load_full_state) ( `state_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">preload_timeline</span>](#method-preload_timeline) ( `timeline_resource`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">start</span>](#method-start) ( `timeline`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `label`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">start_timeline</span>](#method-start_timeline) ( `timeline`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `label_or_idx`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` ) 
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



 Emitted when `paused` changes to true. 

---



<a class="header" id="signal-dialogic_resumed" href="#signal-dialogic_resumed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">dialogic_resumed</span>](#signal-dialogic_resumed) ( )** </a>



 Emitted when `paused` changes to false. 

---



<a class="header" id="signal-event_handled" href="#signal-event_handled">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">event_handled</span>](#signal-event_handled) ( `resource`: [DialogicEvent](class_dialogicevent.md) )** </a>



 Emitted when an event starts being executed. The event may not have finished executing yet. 

---



<a class="header" id="signal-signal_event" href="#signal-signal_event">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">signal_event</span>](#signal-signal_event) ( `argument`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



 Emitted when the `Signal Event` was reached 

---



<a class="header" id="signal-state_changed" href="#signal-state_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">state_changed</span>](#signal-state_changed) ( `new_state`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )** </a>



 Emitted when `current_state` change. 

---



<a class="header" id="signal-text_signal" href="#signal-text_signal">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">text_signal</span>](#signal-text_signal) ( `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 Emitted when `signal` effect was reached in text. 

---



<a class="header" id="signal-timeline_ended" href="#signal-timeline_ended">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">timeline_ended</span>](#signal-timeline_ended) ( )** </a>



 Emitted when dialog ends. This can be a timeline ending or [end_timeline](#property-end_timeline) being called. 

---



<a class="header" id="signal-timeline_started" href="#signal-timeline_started">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">timeline_started</span>](#signal-timeline_started) ( )** </a>



 Emitted when a timeline starts or with either [start](#property-start) or [start_timeline](#property-start_timeline) being invoked. 

---

## Property Descriptions



<a class="header" id="property-animations" href="#property-animations">**<span class="hljs-attribute">var</span> <span class="hljs-title">Animations</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-audio" href="#property-audio">**<span class="hljs-attribute">var</span> <span class="hljs-title">Audio</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-backgrounds" href="#property-backgrounds">**<span class="hljs-attribute">var</span> <span class="hljs-title">Backgrounds</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-choices" href="#property-choices">**<span class="hljs-attribute">var</span> <span class="hljs-title">Choices</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-expressions" href="#property-expressions">**<span class="hljs-attribute">var</span> <span class="hljs-title">Expressions</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-glossary" href="#property-glossary">**<span class="hljs-attribute">var</span> <span class="hljs-title">Glossary</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-history" href="#property-history">**<span class="hljs-attribute">var</span> <span class="hljs-title">History</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-inputs" href="#property-inputs">**<span class="hljs-attribute">var</span> <span class="hljs-title">Inputs</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-jump" href="#property-jump">**<span class="hljs-attribute">var</span> <span class="hljs-title">Jump</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-portraits" href="#property-portraits">**<span class="hljs-attribute">var</span> <span class="hljs-title">Portraits</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-save" href="#property-save">**<span class="hljs-attribute">var</span> <span class="hljs-title">Save</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-settings" href="#property-settings">**<span class="hljs-attribute">var</span> <span class="hljs-title">Settings</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-styles" href="#property-styles">**<span class="hljs-attribute">var</span> <span class="hljs-title">Styles</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text" href="#property-text">**<span class="hljs-attribute">var</span> <span class="hljs-title">Text</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-textinput" href="#property-textinput">**<span class="hljs-attribute">var</span> <span class="hljs-title">TextInput</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-var" href="#property-var">**<span class="hljs-attribute">var</span> <span class="hljs-title">VAR</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-voice" href="#property-voice">**<span class="hljs-attribute">var</span> <span class="hljs-title">Voice</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-current_event_idx" href="#property-current_event_idx">**<span class="hljs-attribute">var</span> <span class="hljs-title">current_event_idx</span> <span style = "color: gray"> = </span> 0** 



Index of the event the timeline handeling is currently at.

---



<a class="header" id="property-current_state" href="#property-current_state">**<span class="hljs-attribute">var</span> <span class="hljs-title">current_state</span> <span style = "color: gray"> = </span> 0** 



Current state (see `States` enum)

---



<a class="header" id="property-current_state_info" href="#property-current_state_info">**<span class="hljs-attribute">var</span> <span class="hljs-title">current_state_info</span> <span style = "color: gray"> = </span> <unknown>** 



Contains all information that subsystems consider relevant for the current situation

---



<a class="header" id="property-current_timeline" href="#property-current_timeline">**<span class="hljs-attribute">var</span> <span class="hljs-title">current_timeline</span> <span style = "color: gray"> = </span> null** 



Reference to the currently executed timeline.

---



<a class="header" id="property-current_timeline_events" href="#property-current_timeline_events">**<span class="hljs-attribute">var</span> <span class="hljs-title">current_timeline_events</span> <span style = "color: gray"> = </span> <unknown>** 



Copy of the `current_timeline`'s events.

---



<a class="header" id="property-paused" href="#property-paused">**<span class="hljs-attribute">var</span> <span class="hljs-title">paused</span> <span style = "color: gray"> = </span> false** 



When `true`, many dialogic processes won't continue until it's false again.

---

## Method Descriptions



<a class="header" id="method-add_subsystem" href="#method-add_subsystem">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_subsystem</span>](#method-add_subsystem) ( `subsystem_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `script_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[DialogicSubsystem](class_dialogicsubsystem.md)</span>** 



Adds a subsystem node with the given `subsystem_name` and `script_path`.

---



<a class="header" id="method-clear" href="#method-clear">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear</span>](#method-clear) ( `clear_flags`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Resets dialogics state fully or partially. By using the clear flags from the `ClearFlags` enum you can specify what info should be kept. For example at timeline end usually it doesn't clear node or subsystem info

---



<a class="header" id="method-end_timeline" href="#method-end_timeline">**<span class="hljs-attribute">func</span> [<span class="hljs-title">end_timeline</span>](#method-end_timeline) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Clears and stops the current timeline.

---



<a class="header" id="method-get_full_state" href="#method-get_full_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_full_state</span>](#method-get_full_state) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Returns a dictionary containing all necessary information to later recreate the same state with load_full_state. The [Save](subsystem_save.md) subsystem might be more useful for you. However, this can be used to integrate the info into your own save system.

---



<a class="header" id="method-get_subsystem" href="#method-get_subsystem">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_subsystem</span>](#method-get_subsystem) ( `subsystem_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[DialogicSubsystem](class_dialogicsubsystem.md)</span>** 



Returns the subsystem node of the given `subsystem_name` or null if it doesn't exist.

---



<a class="header" id="method-handle_event" href="#method-handle_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">handle_event</span>](#method-handle_event) ( `event_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span style = "color: gray">void</span>** 



Handles the event at the given index `event_index`. You can call this manually, but if another event is still executing, it might have unexpected results.

---



<a class="header" id="method-handle_next_event" href="#method-handle_next_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">handle_next_event</span>](#method-handle_next_event) ( `ignore_argument`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



Handles the next event.

---



<a class="header" id="method-has_subsystem" href="#method-has_subsystem">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_subsystem</span>](#method-has_subsystem) ( `subsystem_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns `true` if a subystem with the given `subsystem_name` exists.

---



<a class="header" id="method-load_full_state" href="#method-load_full_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_full_state</span>](#method-load_full_state) ( `state_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span style = "color: gray">void</span>** 



This method tries to load the state from the given `state_info`. Will automatically start a timeline and add a layout if a timeline was running when the dictionary was retrieved with [get_full_state](#property-get_full_state).

---



<a class="header" id="method-preload_timeline" href="#method-preload_timeline">**<span class="hljs-attribute">func</span> [<span class="hljs-title">preload_timeline</span>](#method-preload_timeline) ( `timeline_resource`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



Preloader function, prepares a timeline and returns an object to hold for later `timeline_resource` can be either a path (string) or a loaded timeline (resource)

---



<a class="header" id="method-start" href="#method-start">**<span class="hljs-attribute">func</span> [<span class="hljs-title">start</span>](#method-start) ( `timeline`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `label`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



Method to start a timeline AND ensure that a layout scene is present. For argument info, checkout [start_timeline](#property-start_timeline). -> returns the layout node

---



<a class="header" id="method-start_timeline" href="#method-start_timeline">**<span class="hljs-attribute">func</span> [<span class="hljs-title">start_timeline</span>](#method-start_timeline) ( `timeline`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `label_or_idx`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



Method to start a timeline without adding a layout scene. @timeline can be either a loaded timeline resource or a path to a timeline file. @label_or_idx can be a label (string) or index (int) to skip to immediatly.

---

