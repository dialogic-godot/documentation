
<div class="header-banner purple">
<div class="header-label purple">DialogicVisualEditorFieldNumber</div>
</div>

*This contains the source code documentation of the class `DialogicVisualEditorFieldNumber`.*
        
# DialogicVisualEditorFieldNumber
**Inherits:** [DialogicVisualEditorField](class_dialogicvisualeditorfield.md)

Event block field for integers and floats. Improved version of the native spinbox.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">mode</span>](#property-mode) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">allow_string</span>](#property-allow_string) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">step</span>](#property-step) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.1` 
[<span class="hljs-title">enforce_step</span>](#property-enforce_step) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">min_value</span>](#property-min_value) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `inf_neg` 
[<span class="hljs-title">max_value</span>](#property-max_value) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `inf` 
[<span class="hljs-title">value</span>](#property-value) | [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) |  `0.0` 
[<span class="hljs-title">prefix</span>](#property-prefix) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">suffix</span>](#property-suffix) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span> | [<span class="hljs-title">get_value</span>](#method-get_value) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">use_float_mode</span>](#method-use_float_mode) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">use_int_mode</span>](#method-use_int_mode) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">use_decibel_mode</span>](#method-use_decibel_mode) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_prefix</span>](#method-update_prefix) ( `to_prefix`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_suffix</span>](#method-update_suffix) ( `to_suffix`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
--- 
## Property Descriptions



<a class="header" id="property-mode" href="#property-mode">**<span class="hljs-attribute">var</span> <span class="hljs-title">mode</span> <span style = "color: gray"> = </span> 0** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-allow_string" href="#property-allow_string">**<span class="hljs-attribute">var</span> <span class="hljs-title">allow_string</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-step" href="#property-step">**<span class="hljs-attribute">var</span> <span class="hljs-title">step</span> <span style = "color: gray"> = </span> 0.1** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-enforce_step" href="#property-enforce_step">**<span class="hljs-attribute">var</span> <span class="hljs-title">enforce_step</span> <span style = "color: gray"> = </span> true** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-min_value" href="#property-min_value">**<span class="hljs-attribute">var</span> <span class="hljs-title">min_value</span> <span style = "color: gray"> = </span> inf_neg** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-max_value" href="#property-max_value">**<span class="hljs-attribute">var</span> <span class="hljs-title">max_value</span> <span style = "color: gray"> = </span> inf** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-value" href="#property-value">**<span class="hljs-attribute">var</span> <span class="hljs-title">value</span> <span style = "color: gray"> = </span> 0.0** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-prefix" href="#property-prefix">**<span class="hljs-attribute">var</span> <span class="hljs-title">prefix</span> <span style = "color: gray"> = </span> ""** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-suffix" href="#property-suffix">**<span class="hljs-attribute">var</span> <span class="hljs-title">suffix</span> <span style = "color: gray"> = </span> ""** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-get_value" href="#method-get_value">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_value</span>](#method-get_value) ( )</a>  ⇒ <span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-use_float_mode" href="#method-use_float_mode">**<span class="hljs-attribute">func</span> [<span class="hljs-title">use_float_mode</span>](#method-use_float_mode) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-use_int_mode" href="#method-use_int_mode">**<span class="hljs-attribute">func</span> [<span class="hljs-title">use_int_mode</span>](#method-use_int_mode) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-use_decibel_mode" href="#method-use_decibel_mode">**<span class="hljs-attribute">func</span> [<span class="hljs-title">use_decibel_mode</span>](#method-use_decibel_mode) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_prefix" href="#method-update_prefix">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_prefix</span>](#method-update_prefix) ( `to_prefix`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_suffix" href="#method-update_suffix">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_suffix</span>](#method-update_suffix) ( `to_suffix`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

