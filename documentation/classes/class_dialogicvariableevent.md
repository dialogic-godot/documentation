
<div class="header-banner purple">
<div class="header-label purple">DialogicVariableEvent</div>
</div>

*This contains the source code documentation of the class `DialogicVariableEvent`.*
        
# DialogicVariableEvent
**Inherits:** DialogicEvent

Settings
## Properties
Name | Type | Default 
--- | --- | --- 
name | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
operation | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
random_max | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `100` 
random_min | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
value | [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) |  `""` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">from_text</span>](#property-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_value_suggestions</span>](#property-get_value_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_var_suggestions</span>](#property-get_var_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">is_valid_event</span>](#property-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">to_text</span>](#property-to_text) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">update_editor_warning</span>](#property-update_editor_warning) ( ) 
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



<a class="header" id="property-build_event_editor" href="#property-build_event_editor">**<span class="hljs-attribute">void</span> [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-from_text" href="#property-from_text">**<span class="hljs-attribute">void</span> [<span class="hljs-title">from_text</span>](#property-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_value_suggestions" href="#property-get_value_suggestions">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_value_suggestions</span>](#property-get_value_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_var_suggestions" href="#property-get_var_suggestions">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_var_suggestions</span>](#property-get_var_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_valid_event" href="#property-is_valid_event">**<span class="hljs-attribute">void</span> [<span class="hljs-title">is_valid_event</span>](#property-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-to_text" href="#property-to_text">**<span class="hljs-attribute">void</span> [<span class="hljs-title">to_text</span>](#property-to_text) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-update_editor_warning" href="#property-update_editor_warning">**<span class="hljs-attribute">void</span> [<span class="hljs-title">update_editor_warning</span>](#property-update_editor_warning) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

