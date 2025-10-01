
<div class="header-banner purple">
<div class="header-label purple">Jump</div>
</div>

*This contains the source code documentation of the class `subsystem_Jump`.*
        
# subsystem_Jump
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that holds methods for jumping to specific labels, or return to the previous jump.
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `_load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">jump_to_label</span>](#method-jump_to_label) ( `label`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">push_to_jump_stack</span>](#method-push_to_jump_stack) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume_from_last_jump</span>](#method-resume_from_last_jump) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_jump_stack_empty</span>](#method-is_jump_stack_empty) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_last_label_identifier</span>](#method-get_last_label_identifier) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_last_label_name</span>](#method-get_last_label_name) ( ) 
--- 

## Signals


<a class="header" id="signal-switched_timeline" href="#signal-switched_timeline">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">switched_timeline</span>](#signal-switched_timeline) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-jumped_to_label" href="#signal-jumped_to_label">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">jumped_to_label</span>](#signal-jumped_to_label) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 Emitted when a jump event jumps to a label. Gives a dictionary witht the keys: 
Key         | Value Type              | Value 
----------- | ----------------------- | ----- 
`timeline`  | [DialogicTimeline](class_dialogictimeline.md) | The timeline we are in now. 
`label`     | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)           | The label we went to (empty if beginning). 
 

---



<a class="header" id="signal-returned_from_jump" href="#signal-returned_from_jump">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">returned_from_jump</span>](#signal-returned_from_jump) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 Emitted when a return event is hit and there was a timeline to return to. Gives a dictionary witht the keys: 
Key             | Value Type              | Value 
--------------- | ----------------------- | ----- 
`sub_timeline`  | [DialogicTimeline](class_dialogictimeline.md) | The timeline we were in before. 
`label`         | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)           | The label we went back to (empty if beginning). 
 

---



<a class="header" id="signal-passed_label" href="#signal-passed_label">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">passed_label</span>](#signal-passed_label) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 Emitted when a label event is executed (usually does nothing else). Gives a dictionary witht the keys: 
Key                 | Value Type              | Value 
------------------- | ----------------------- | ----- 
`identifier`        | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)           | The identifier of the label event. 
`display_name`      | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)           | The display name, possibly translated. 
`display_name_orig` | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)           | The untranslated display name. 
`timeline`          | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)           | The identifier of the timeline we are in. 
 

---

## Method Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-load_game_state" href="#method-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `_load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-jump_to_label" href="#method-jump_to_label">**<span class="hljs-attribute">func</span> [<span class="hljs-title">jump_to_label</span>](#method-jump_to_label) ( `label`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-push_to_jump_stack" href="#method-push_to_jump_stack">**<span class="hljs-attribute">func</span> [<span class="hljs-title">push_to_jump_stack</span>](#method-push_to_jump_stack) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-resume_from_last_jump" href="#method-resume_from_last_jump">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume_from_last_jump</span>](#method-resume_from_last_jump) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_jump_stack_empty" href="#method-is_jump_stack_empty">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_jump_stack_empty</span>](#method-is_jump_stack_empty) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_last_label_identifier" href="#method-get_last_label_identifier">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_last_label_identifier</span>](#method-get_last_label_identifier) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the identifier name of the last passed label

---



<a class="header" id="method-get_last_label_name" href="#method-get_last_label_name">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_last_label_name</span>](#method-get_last_label_name) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the display name of the last passed label (translated if translation are enabled)

---

