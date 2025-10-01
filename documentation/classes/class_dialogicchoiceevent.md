
<div class="header-banner purple">
<div class="header-label purple">DialogicChoiceEvent</div>
</div>

*This contains the source code documentation of the class `DialogicChoiceEvent`.*
        
# DialogicChoiceEvent
**Inherits:** [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource)

Event that allows adding choices. Needs to go after a text event (or another choices EndBranch).
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">text</span>](#property-text) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">condition</span>](#property-condition) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">else_action</span>](#property-else_action) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `2` 
[<span class="hljs-title">disabled_text</span>](#property-disabled_text) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">extra_data</span>](#property-extra_data) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{}` 
[<span class="hljs-title">regex</span>](#property-regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |  `create_from_string(...)` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">to_text</span>](#method-to_text) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">allow_alt_text</span>](#method-allow_alt_text) ( ) 
--- 
## Constants


<a class="header" id="constant-HIDE" href="#constant-HIDE">**<span class="hljs-attribute">const</span> <span class="hljs-title">HIDE</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-DISABLE" href="#constant-DISABLE">**<span class="hljs-attribute">const</span> <span class="hljs-title">DISABLE</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-DEFAULT" href="#constant-DEFAULT">**<span class="hljs-attribute">const</span> <span class="hljs-title">DEFAULT</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-text" href="#property-text">**<span class="hljs-attribute">var</span> <span class="hljs-title">text</span> <span style = "color: gray"> = </span> ""** 



# Settings The text that is displayed on the choice button.

---



<a class="header" id="property-condition" href="#property-condition">**<span class="hljs-attribute">var</span> <span class="hljs-title">condition</span> <span style = "color: gray"> = </span> ""** 



If not empty this condition will determine if this choice is active.

---



<a class="header" id="property-else_action" href="#property-else_action">**<span class="hljs-attribute">var</span> <span class="hljs-title">else_action</span> <span style = "color: gray"> = </span> 2** 



Determines what happens if   is false. Default will use the action set in the settings.

---



<a class="header" id="property-disabled_text" href="#property-disabled_text">**<span class="hljs-attribute">var</span> <span class="hljs-title">disabled_text</span> <span style = "color: gray"> = </span> ""** 



The text that is displayed if  is false and  is Disable. If empty  will be used for disabled button as well.

---



<a class="header" id="property-extra_data" href="#property-extra_data">**<span class="hljs-attribute">var</span> <span class="hljs-title">extra_data</span> <span style = "color: gray"> = </span> {}** 



A dictionary that can be filled with arbitrary information This can then be interpreted by a custom choice layer

---



<a class="header" id="property-regex" href="#property-regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">regex</span> <span style = "color: gray"> = </span> create_from_string(...)** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-to_text" href="#method-to_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">to_text</span>](#method-to_text) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-from_text" href="#method-from_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode_parameters" href="#method-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_valid_event" href="#method-is_valid_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-allow_alt_text" href="#method-allow_alt_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">allow_alt_text</span>](#method-allow_alt_text) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

