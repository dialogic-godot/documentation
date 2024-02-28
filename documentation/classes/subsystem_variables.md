
<div class="header-banner purple">
<div class="header-label purple">subsystem_Variables</div>
</div>

*This contains the source code documentation of the class `subsystem_Variables`.*
        
# subsystem_Variables
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that manages variables and allows to access them.
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">folders</span>](#property-folders) ( ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_autoloads</span>](#property-get_autoloads) ( ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">get_variable</span>](#property-get_variable) ( `variable_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has</span>](#property-has) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#property-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">merge_folder</span>](#property-merge_folder) ( `new`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `defs`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">parse_variables</span>](#property-parse_variables) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset</span>](#property-reset) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">set_variable</span>](#property-set_variable) ( `variable_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">variables</span>](#property-variables) ( `absolute`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
--- 

## Signals


<a class="header" id="signal-variable_changed" href="#signal-variable_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">variable_changed</span>](#signal-variable_changed) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



Emitted if a dialogic variable changes

---



<a class="header" id="signal-variable_was_set" href="#signal-variable_was_set">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">variable_was_set</span>](#signal-variable_was_set) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



Emitted on any set variable event

---

## Method Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-folders" href="#method-folders">**<span class="hljs-attribute">func</span> [<span class="hljs-title">folders</span>](#property-folders) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_autoloads" href="#method-get_autoloads">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_autoloads</span>](#property-get_autoloads) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_variable" href="#method-get_variable">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_variable</span>](#property-get_variable) ( `variable_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null` )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-has" href="#method-has">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has</span>](#property-has) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns true if a variable with the given path exists

---



<a class="header" id="method-load_game_state" href="#method-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#property-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-merge_folder" href="#method-merge_folder">**<span class="hljs-attribute">func</span> [<span class="hljs-title">merge_folder</span>](#property-merge_folder) ( `new`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `defs`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-parse_variables" href="#method-parse_variables">**<span class="hljs-attribute">func</span> [<span class="hljs-title">parse_variables</span>](#property-parse_variables) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



This function will try to get the value of variables provided inside curly brackets and replace them with their values. It will: - look for the strings to replace - search all autoloads - try to get the value from context  So if you provide a string like `Hello, how are you doing {Game.player_name} it will try to search for an autoload with the name `Game` and get the value of `player_name` to replace it.

---



<a class="header" id="method-reset" href="#method-reset">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset</span>](#property-reset) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



Resets all variables or a specific variable to the value(s) defined in the variable editor

---



<a class="header" id="method-set_variable" href="#method-set_variable">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_variable</span>](#property-set_variable) ( `variable_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-variables" href="#method-variables">**<span class="hljs-attribute">func</span> [<span class="hljs-title">variables</span>](#property-variables) ( `absolute`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

