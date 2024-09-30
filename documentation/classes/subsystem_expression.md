
<div class="header-banner purple">
<div class="header-label purple">Expression</div>
</div>

*This contains the source code documentation of the class `subsystem_Expression`.*
        
# subsystem_Expression
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

##################################################################################################
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">condition_modifier_regex</span>](#property-condition_modifier_regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |  `create_from_string(...)` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">execute_string</span>](#method-execute_string) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null`, `no_warning`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">execute_condition</span>](#method-execute_condition) ( `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">modifier_condition</span>](#method-modifier_condition) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">d_range</span>](#method-d_range) ( `a1`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `a2`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null`, `a3`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null`, `a4`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null` ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">d_len</span>](#method-d_len) ( `arg`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">d_regex</span>](#method-d_regex) ( `input`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `pattern`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `offset`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0`, `end`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `-1` ) 
--- 
## Property Descriptions



<a class="header" id="property-condition_modifier_regex" href="#property-condition_modifier_regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">condition_modifier_regex</span> <span style = "color: gray"> = </span> create_from_string(...)** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-execute_string" href="#method-execute_string">**<span class="hljs-attribute">func</span> [<span class="hljs-title">execute_string</span>](#method-execute_string) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null`, `no_warning`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-execute_condition" href="#method-execute_condition">**<span class="hljs-attribute">func</span> [<span class="hljs-title">execute_condition</span>](#method-execute_condition) ( `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-modifier_condition" href="#method-modifier_condition">**<span class="hljs-attribute">func</span> [<span class="hljs-title">modifier_condition</span>](#method-modifier_condition) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-d_range" href="#method-d_range">**<span class="hljs-attribute">func</span> [<span class="hljs-title">d_range</span>](#method-d_range) ( `a1`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `a2`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null`, `a3`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null`, `a4`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null` )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



##################################################################################################

---



<a class="header" id="method-d_len" href="#method-d_len">**<span class="hljs-attribute">func</span> [<span class="hljs-title">d_len</span>](#method-d_len) ( `arg`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-d_regex" href="#method-d_regex">**<span class="hljs-attribute">func</span> [<span class="hljs-title">d_regex</span>](#method-d_regex) ( `input`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `pattern`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `offset`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0`, `end`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `-1` )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

