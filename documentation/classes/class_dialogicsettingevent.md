
<div class="header-banner purple">
<div class="header-label purple">DialogicSettingEvent</div>
</div>

*This contains the source code documentation of the class `DialogicSettingEvent`.*
        
# DialogicSettingEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

# Settings
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">name</span>](#property-name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">value</span>](#property-value) | [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) |  `""` 
[<span class="hljs-title">mode</span>](#property-mode) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">to_text</span>](#method-to_text) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_settings_suggestions</span>](#method-get_settings_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_value_suggestions</span>](#method-get_value_suggestions) ( `_filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
--- 
## Constants


<a class="header" id="constant-SET" href="#constant-SET">**<span class="hljs-attribute">const</span> <span class="hljs-title">SET</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-RESET" href="#constant-RESET">**<span class="hljs-attribute">const</span> <span class="hljs-title">RESET</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-RESET_ALL" href="#constant-RESET_ALL">**<span class="hljs-attribute">const</span> <span class="hljs-title">RESET_ALL</span><span class="hljs-comment"> = 2</span>**</a>



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


<a class="header" id="constant-EXPRESSION" href="#constant-EXPRESSION">**<span class="hljs-attribute">const</span> <span class="hljs-title">EXPRESSION</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-name" href="#property-name">**<span class="hljs-attribute">var</span> <span class="hljs-title">name</span> <span style = "color: gray"> = </span> ""** 



The name of the setting to save to.

---



<a class="header" id="property-value" href="#property-value">**<span class="hljs-attribute">var</span> <span class="hljs-title">value</span> <span style = "color: gray"> = </span> ""** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-mode" href="#property-mode">**<span class="hljs-attribute">var</span> <span class="hljs-title">mode</span> <span style = "color: gray"> = </span> 0** 



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



<a class="header" id="method-get_settings_suggestions" href="#method-get_settings_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_settings_suggestions</span>](#method-get_settings_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_value_suggestions" href="#method-get_value_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_value_suggestions</span>](#method-get_value_suggestions) ( `_filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

