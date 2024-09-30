
<div class="header-banner purple">
<div class="header-label purple">DialogicVariableEvent</div>
</div>

*This contains the source code documentation of the class `DialogicVariableEvent`.*
        
# DialogicVariableEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

Settings
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">name</span>](#property-name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">operation</span>](#property-operation) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">value</span>](#property-value) | [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) |  `""` 
[<span class="hljs-title">random_min</span>](#property-random_min) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">random_max</span>](#property-random_max) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `100` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">to_text</span>](#method-to_text) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_var_suggestions</span>](#method-get_var_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_value_suggestions</span>](#method-get_value_suggestions) ( `_filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_editor_warning</span>](#method-update_editor_warning) ( ) 
--- 
## Constants


<a class="header" id="constant-SET" href="#constant-SET">**<span class="hljs-attribute">const</span> <span class="hljs-title">SET</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ADD" href="#constant-ADD">**<span class="hljs-attribute">const</span> <span class="hljs-title">ADD</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-SUBSTRACT" href="#constant-SUBSTRACT">**<span class="hljs-attribute">const</span> <span class="hljs-title">SUBSTRACT</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-MULTIPLY" href="#constant-MULTIPLY">**<span class="hljs-attribute">const</span> <span class="hljs-title">MULTIPLY</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-DIVIDE" href="#constant-DIVIDE">**<span class="hljs-attribute">const</span> <span class="hljs-title">DIVIDE</span><span class="hljs-comment"> = 4</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-STRING" href="#constant-STRING">**<span class="hljs-attribute">const</span> <span class="hljs-title">STRING</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-NUMBER" href="#constant-NUMBER">**<span class="hljs-attribute">const</span> <span class="hljs-title">NUMBER</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-VARIABLE" href="#constant-VARIABLE">**<span class="hljs-attribute">const</span> <span class="hljs-title">VARIABLE</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-BOOL" href="#constant-BOOL">**<span class="hljs-attribute">const</span> <span class="hljs-title">BOOL</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-EXPRESSION" href="#constant-EXPRESSION">**<span class="hljs-attribute">const</span> <span class="hljs-title">EXPRESSION</span><span class="hljs-comment"> = 4</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-RANDOM_NUMBER" href="#constant-RANDOM_NUMBER">**<span class="hljs-attribute">const</span> <span class="hljs-title">RANDOM_NUMBER</span><span class="hljs-comment"> = 5</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-name" href="#property-name">**<span class="hljs-attribute">var</span> <span class="hljs-title">name</span> <span style = "color: gray"> = </span> ""** 



Name/Path of the variable that should be changed.

---



<a class="header" id="property-operation" href="#property-operation">**<span class="hljs-attribute">var</span> <span class="hljs-title">operation</span> <span style = "color: gray"> = </span> 0** 



The operation to perform.

---



<a class="header" id="property-value" href="#property-value">**<span class="hljs-attribute">var</span> <span class="hljs-title">value</span> <span style = "color: gray"> = </span> ""** 



The value that is used. Can be a variable as well.

---



<a class="header" id="property-random_min" href="#property-random_min">**<span class="hljs-attribute">var</span> <span class="hljs-title">random_min</span> <span style = "color: gray"> = </span> 0** 



If true, a random number between  and  is used instead of .

---



<a class="header" id="property-random_max" href="#property-random_max">**<span class="hljs-attribute">var</span> <span class="hljs-title">random_max</span> <span style = "color: gray"> = </span> 100** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-to_text" href="#method-to_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">to_text</span>](#method-to_text) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-from_text" href="#method-from_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_valid_event" href="#method-is_valid_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_var_suggestions" href="#method-get_var_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_var_suggestions</span>](#method-get_var_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_value_suggestions" href="#method-get_value_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_value_suggestions</span>](#method-get_value_suggestions) ( `_filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_editor_warning" href="#method-update_editor_warning">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_editor_warning</span>](#method-update_editor_warning) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

