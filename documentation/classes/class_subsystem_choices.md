
<div class="header-banner purple">
<div class="header-label purple">subsystem_choices</div>
</div>

*This contains the source code documentation of the class `subsystem_choices`.*
        
# subsystem_choices
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that manages showing and activating of choices.
## Properties
Name | Type | Default 
--- | --- | --- 
choice_blocker | [Timer](https://docs.godotengine.org/en/latest/classes/class_timer.html#class-timer) |   
last_question_info | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_current_choice_indexes</span>](#property-get_current_choice_indexes) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">hide_all_choices</span>](#property-hide_all_choices) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_question</span>](#property-is_question) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">show_choice</span>](#property-show_choice) ( `button_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `event_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">show_current_choices</span>](#property-show_current_choices) ( `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
--- 

## Signals


<a class="header" id="signal-choice_selected" href="#signal-choice_selected">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">choice_selected</span>](#signal-choice_selected) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-choices_shown" href="#signal-choices_shown">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">choices_shown</span>](#signal-choices_shown) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-clear_game_state" href="#property-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_current_choice_indexes" href="#property-get_current_choice_indexes">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_current_choice_indexes</span>](#property-get_current_choice_indexes) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-hide_all_choices" href="#property-hide_all_choices">**<span class="hljs-attribute">func</span> [<span class="hljs-title">hide_all_choices</span>](#property-hide_all_choices) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Hides all choice buttons.

---



<a class="header" id="property-is_question" href="#property-is_question">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_question</span>](#property-is_question) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-show_choice" href="#property-show_choice">**<span class="hljs-attribute">func</span> [<span class="hljs-title">show_choice</span>](#property-show_choice) ( `button_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `event_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span style = "color: gray">void</span>** 



Adds a button with the given text that leads to the given event.

---



<a class="header" id="property-show_current_choices" href="#property-show_current_choices">**<span class="hljs-attribute">func</span> [<span class="hljs-title">show_current_choices</span>](#property-show_current_choices) ( `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span style = "color: gray">void</span>** 



Lists all current choices and shows buttons.

---

