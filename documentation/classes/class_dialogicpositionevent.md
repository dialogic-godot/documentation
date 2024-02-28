
<div class="header-banner purple">
<div class="header-label purple">DialogicPositionEvent</div>
</div>

*This contains the source code documentation of the class `DialogicPositionEvent`.*
        
# DialogicPositionEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

# Settings
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">action</span>](#property-action) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">movement_time</span>](#property-movement_time) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
[<span class="hljs-title">position</span>](#property-position) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">vector</span>](#property-vector) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |  `Vector2(0, 0)` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_shortcode</span>](#property-get_shortcode) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( ) 
--- 
## Constants


<a class="header" id="constant-SET_RELATIVE" href="#constant-SET_RELATIVE">**<span class="hljs-attribute">const</span> <span class="hljs-title">SET_RELATIVE</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-SET_ABSOLUTE" href="#constant-SET_ABSOLUTE">**<span class="hljs-attribute">const</span> <span class="hljs-title">SET_ABSOLUTE</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-RESET" href="#constant-RESET">**<span class="hljs-attribute">const</span> <span class="hljs-title">RESET</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-RESET_ALL" href="#constant-RESET_ALL">**<span class="hljs-attribute">const</span> <span class="hljs-title">RESET_ALL</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-action" href="#property-action">**<span class="hljs-attribute">var</span> <span class="hljs-title">action</span> <span style = "color: gray"> = </span> 0** 



The type of action: SetRelative, SetAbsolute, Reset, ResetAll

---



<a class="header" id="property-movement_time" href="#property-movement_time">**<span class="hljs-attribute">var</span> <span class="hljs-title">movement_time</span> <span style = "color: gray"> = </span> 0.0** 



The time the tweening will take.

---



<a class="header" id="property-position" href="#property-position">**<span class="hljs-attribute">var</span> <span class="hljs-title">position</span> <span style = "color: gray"> = </span> 0** 



The position that should be affected

---



<a class="header" id="property-vector" href="#property-vector">**<span class="hljs-attribute">var</span> <span class="hljs-title">vector</span> <span style = "color: gray"> = </span> Vector2(0, 0)** 



A vector representing a relative change or an absolute position (for SetRelative and SetAbsolute)

---

## Method Descriptions



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode" href="#method-get_shortcode">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode</span>](#property-get_shortcode) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode_parameters" href="#method-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

