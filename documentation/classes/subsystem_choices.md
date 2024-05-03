
<div class="header-banner purple">
<div class="header-label purple">Choices</div>
</div>

*This contains the source code documentation of the class `subsystem_Choices`.*
        
# subsystem_Choices
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that manages showing and activating of choices.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">autofocus_first_choice</span>](#property-autofocus_first_choice) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">block_delay</span>](#property-block_delay) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.2` 
[<span class="hljs-title">default_false_behaviour</span>](#property-default_false_behaviour) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">hotkey_behaviour</span>](#property-hotkey_behaviour) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">last_question_info</span>](#property-last_question_info) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">reveal_by_input</span>](#property-reveal_by_input) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">reveal_delay</span>](#property-reveal_delay) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_current_choice_indexes</span>](#method-get_current_choice_indexes) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">hide_all_choices</span>](#method-hide_all_choices) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_question</span>](#method-is_question) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">show_choice</span>](#method-show_choice) ( `button_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `event_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">show_current_choices</span>](#method-show_current_choices) ( `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
--- 
## Constants


<a class="header" id="constant-HIDE" href="#constant-HIDE">**<span class="hljs-attribute">const</span> <span class="hljs-title">HIDE</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-DISABLE" href="#constant-DISABLE">**<span class="hljs-attribute">const</span> <span class="hljs-title">DISABLE</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-NONE" href="#constant-NONE">**<span class="hljs-attribute">const</span> <span class="hljs-title">NONE</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-NUMBERS" href="#constant-NUMBERS">**<span class="hljs-attribute">const</span> <span class="hljs-title">NUMBERS</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-choice_selected" href="#signal-choice_selected">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">choice_selected</span>](#signal-choice_selected) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 Emitted when a choice button was pressed. Info includes the keys 'button_index', 'text', 'event_index'. 

---



<a class="header" id="signal-choices_shown" href="#signal-choices_shown">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">choices_shown</span>](#signal-choices_shown) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 Emitted when a set of choices is reached and shown. Info includes the keys 'choices' (an array of dictionaries with infos on all the choices). 

---

## Property Descriptions



<a class="header" id="property-autofocus_first_choice" href="#property-autofocus_first_choice">**<span class="hljs-attribute">var</span> <span class="hljs-title">autofocus_first_choice</span> <span style = "color: gray"> = </span> true** 



If true, the first (top-most) choice will be focused

---



<a class="header" id="property-block_delay" href="#property-block_delay">**<span class="hljs-attribute">var</span> <span class="hljs-title">block_delay</span> <span style = "color: gray"> = </span> 0.2** 



The delay between the choices becoming visible and being clickable. Can prevent accidental selection.

---



<a class="header" id="property-default_false_behaviour" href="#property-default_false_behaviour">**<span class="hljs-attribute">var</span> <span class="hljs-title">default_false_behaviour</span> <span style = "color: gray"> = </span> 0** 



The behaviour of choices with a false condition and else_action set to DEFAULT.

---



<a class="header" id="property-hotkey_behaviour" href="#property-hotkey_behaviour">**<span class="hljs-attribute">var</span> <span class="hljs-title">hotkey_behaviour</span> <span style = "color: gray"> = </span> 0** 



Will add some hotkeys to the choices if different then HotkeyBehaviour.NONE.

---



<a class="header" id="property-last_question_info" href="#property-last_question_info">**<span class="hljs-attribute">var</span> <span class="hljs-title">last_question_info</span> <span style = "color: gray"> = </span> <unknown>** 



Contains information on the latest question.

---



<a class="header" id="property-reveal_by_input" href="#property-reveal_by_input">**<span class="hljs-attribute">var</span> <span class="hljs-title">reveal_by_input</span> <span style = "color: gray"> = </span> false** 



If true the player has to click to reveal choices when they are reached

---



<a class="header" id="property-reveal_delay" href="#property-reveal_delay">**<span class="hljs-attribute">var</span> <span class="hljs-title">reveal_delay</span> <span style = "color: gray"> = </span> 0.0** 



The delay between the text finishing revealing and the choices appearing

---

## Method Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_current_choice_indexes" href="#method-get_current_choice_indexes">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_current_choice_indexes</span>](#method-get_current_choice_indexes) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-hide_all_choices" href="#method-hide_all_choices">**<span class="hljs-attribute">func</span> [<span class="hljs-title">hide_all_choices</span>](#method-hide_all_choices) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Hides all choice buttons.

---



<a class="header" id="method-is_question" href="#method-is_question">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_question</span>](#method-is_question) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-show_choice" href="#method-show_choice">**<span class="hljs-attribute">func</span> [<span class="hljs-title">show_choice</span>](#method-show_choice) ( `button_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `event_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span style = "color: gray">void</span>** 



Adds a button with the given text that leads to the given event.

---



<a class="header" id="method-show_current_choices" href="#method-show_current_choices">**<span class="hljs-attribute">func</span> [<span class="hljs-title">show_current_choices</span>](#method-show_current_choices) ( `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span style = "color: gray">void</span>** 



Lists all current choices and shows buttons.

---

