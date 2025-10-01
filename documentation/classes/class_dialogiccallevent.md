
<div class="header-banner purple">
<div class="header-label purple">DialogicCallEvent</div>
</div>

*This contains the source code documentation of the class `DialogicCallEvent`.*
        
# DialogicCallEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

Event that allows calling a method in a node or autoload.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">autoload_name</span>](#property-autoload_name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">method</span>](#property-method) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">arguments</span>](#property-arguments) | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |  `[]` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">to_text</span>](#method-to_text) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_method_suggestions</span>](#method-get_method_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_argument_info</span>](#method-update_argument_info) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">check_arguments_and_update_warning</span>](#method-check_arguments_and_update_warning) ( ) 
--- 
## Property Descriptions



<a class="header" id="property-autoload_name" href="#property-autoload_name">**<span class="hljs-attribute">var</span> <span class="hljs-title">autoload_name</span> <span style = "color: gray"> = </span> ""** 



The name of the autoload to call the method on.

---



<a class="header" id="property-method" href="#property-method">**<span class="hljs-attribute">var</span> <span class="hljs-title">method</span> <span style = "color: gray"> = </span> ""** 



The name of the method to call on the given autoload.

---



<a class="header" id="property-arguments" href="#property-arguments">**<span class="hljs-attribute">var</span> <span class="hljs-title">arguments</span> <span style = "color: gray"> = </span> []** 



A list of arguments to give to the call.

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



<a class="header" id="method-get_shortcode_parameters" href="#method-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_method_suggestions" href="#method-get_method_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_method_suggestions</span>](#method-get_method_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_argument_info" href="#method-update_argument_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_argument_info</span>](#method-update_argument_info) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-check_arguments_and_update_warning" href="#method-check_arguments_and_update_warning">**<span class="hljs-attribute">func</span> [<span class="hljs-title">check_arguments_and_update_warning</span>](#method-check_arguments_and_update_warning) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

