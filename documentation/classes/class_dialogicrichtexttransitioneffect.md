
<div class="header-banner purple">
<div class="header-label purple">DialogicRichTextTransitionEffect</div>
</div>

*This contains the source code documentation of the class `DialogicRichTextTransitionEffect`.*
        
# DialogicRichTextTransitionEffect
**Inherits:** [RichTextEffect](https://docs.godotengine.org/en/latest/classes/class_richtexteffect.html#class-richtexteffect)


## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">visible_characters</span>](#property-visible_characters) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `-1` 
[<span class="hljs-title">bbcode</span>](#property-bbcode) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"animate_in"` 
[<span class="hljs-title">cache</span>](#property-cache) | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |  `[]` 
[<span class="hljs-title">time</span>](#property-time) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.2` 
[<span class="hljs-title">color_modulate</span>](#property-color_modulate) | [Gradient](https://docs.godotengine.org/en/latest/classes/class_gradient.html#class-gradient) |  `null` 
[<span class="hljs-title">color_replace</span>](#property-color_replace) | [Gradient](https://docs.godotengine.org/en/latest/classes/class_gradient.html#class-gradient) |  `null` 
[<span class="hljs-title">scale_enabled</span>](#property-scale_enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">scale_curve</span>](#property-scale_curve) | [Curve](https://docs.godotengine.org/en/latest/classes/class_curve.html#class-curve) |  `new()` 
[<span class="hljs-title">scale_pivot</span>](#property-scale_pivot) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |  `Vector2(0, 0)` 
[<span class="hljs-title">position_enabled</span>](#property-position_enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">position_x_curve</span>](#property-position_x_curve) | [Curve](https://docs.godotengine.org/en/latest/classes/class_curve.html#class-curve) |  `new()` 
[<span class="hljs-title">position_y_curve</span>](#property-position_y_curve) | [Curve](https://docs.godotengine.org/en/latest/classes/class_curve.html#class-curve) |  `new()` 
[<span class="hljs-title">test_value</span>](#property-test_value) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `-0.1` 
[<span class="hljs-title">was_skipped</span>](#property-was_skipped) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">was_reset</span>](#property-was_reset) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset</span>](#method-reset) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">skip</span>](#method-skip) ( ) 
--- 
## Property Descriptions



<a class="header" id="property-visible_characters" href="#property-visible_characters">**<span class="hljs-attribute">var</span> <span class="hljs-title">visible_characters</span> <span style = "color: gray"> = </span> -1** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-bbcode" href="#property-bbcode">**<span class="hljs-attribute">var</span> <span class="hljs-title">bbcode</span> <span style = "color: gray"> = </span> "animate_in"** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-cache" href="#property-cache">**<span class="hljs-attribute">var</span> <span class="hljs-title">cache</span> <span style = "color: gray"> = </span> []** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-time" href="#property-time">**<span class="hljs-attribute">var</span> <span class="hljs-title">time</span> <span style = "color: gray"> = </span> 0.2** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-color_modulate" href="#property-color_modulate">**<span class="hljs-attribute">var</span> <span class="hljs-title">color_modulate</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-color_replace" href="#property-color_replace">**<span class="hljs-attribute">var</span> <span class="hljs-title">color_replace</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-scale_enabled" href="#property-scale_enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">scale_enabled</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-scale_curve" href="#property-scale_curve">**<span class="hljs-attribute">var</span> <span class="hljs-title">scale_curve</span> <span style = "color: gray"> = </span> new()** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-scale_pivot" href="#property-scale_pivot">**<span class="hljs-attribute">var</span> <span class="hljs-title">scale_pivot</span> <span style = "color: gray"> = </span> Vector2(0, 0)** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-position_enabled" href="#property-position_enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">position_enabled</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-position_x_curve" href="#property-position_x_curve">**<span class="hljs-attribute">var</span> <span class="hljs-title">position_x_curve</span> <span style = "color: gray"> = </span> new()** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-position_y_curve" href="#property-position_y_curve">**<span class="hljs-attribute">var</span> <span class="hljs-title">position_y_curve</span> <span style = "color: gray"> = </span> new()** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-test_value" href="#property-test_value">**<span class="hljs-attribute">var</span> <span class="hljs-title">test_value</span> <span style = "color: gray"> = </span> -0.1** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-was_skipped" href="#property-was_skipped">**<span class="hljs-attribute">var</span> <span class="hljs-title">was_skipped</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-was_reset" href="#property-was_reset">**<span class="hljs-attribute">var</span> <span class="hljs-title">was_reset</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-reset" href="#method-reset">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset</span>](#method-reset) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-skip" href="#method-skip">**<span class="hljs-attribute">func</span> [<span class="hljs-title">skip</span>](#method-skip) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

