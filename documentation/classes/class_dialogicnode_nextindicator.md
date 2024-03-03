
<div class="header-banner purple">
<div class="header-label purple">DialogicNode_NextIndicator</div>
</div>

*This contains the source code documentation of the class `DialogicNode_NextIndicator`.*
        
# DialogicNode_NextIndicator
**Inherits:** [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)

Node that is shown when the text is fully revealed. The default implementation allows to set an icon and animation.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">animation</span>](#property-animation) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">enabled</span>](#property-enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">show_on_autoadvance</span>](#property-show_on_autoadvance) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">show_on_questions</span>](#property-show_on_questions) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">texture</span>](#property-texture) | [Texture2D](https://docs.godotengine.org/en/latest/classes/class_texture2d.html#class-texture2d) |   
[<span class="hljs-title">texture_rect</span>](#property-texture_rect) | [TextureRect](https://docs.godotengine.org/en/latest/classes/class_texturerect.html#class-texturerect) |   
[<span class="hljs-title">texture_size</span>](#property-texture_size) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |  `Vector2(32, 32)` 
[<span class="hljs-title">tween</span>](#property-tween) | [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">play_animation</span>](#method-play_animation) ( `animation`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) ) 
--- 
## Property Descriptions



<a class="header" id="property-animation" href="#property-animation">**<span class="hljs-attribute">var</span> <span class="hljs-title">animation</span> <span style = "color: gray"> = </span> 0** 



What animation should the indicator do.

---



<a class="header" id="property-enabled" href="#property-enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">enabled</span> <span style = "color: gray"> = </span> true** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-show_on_autoadvance" href="#property-show_on_autoadvance">**<span class="hljs-attribute">var</span> <span class="hljs-title">show_on_autoadvance</span> <span style = "color: gray"> = </span> false** 



If true the next indicator will be shown even if dialogic will autocontinue.

---



<a class="header" id="property-show_on_questions" href="#property-show_on_questions">**<span class="hljs-attribute">var</span> <span class="hljs-title">show_on_questions</span> <span style = "color: gray"> = </span> false** 



If true the next indicator will also be shown if the text is a question.

---



<a class="header" id="property-texture" href="#property-texture">**<span class="hljs-attribute">var</span> <span class="hljs-title">texture</span> <span style = "color: gray"> = </span> <unknown>** 



Set the image to use as the indicator.

---



<a class="header" id="property-texture_rect" href="#property-texture_rect">**<span class="hljs-attribute">var</span> <span class="hljs-title">texture_rect</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-texture_size" href="#property-texture_size">**<span class="hljs-attribute">var</span> <span class="hljs-title">texture_size</span> <span style = "color: gray"> = </span> Vector2(32, 32)** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-tween" href="#property-tween">**<span class="hljs-attribute">var</span> <span class="hljs-title">tween</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-play_animation" href="#method-play_animation">**<span class="hljs-attribute">func</span> [<span class="hljs-title">play_animation</span>](#method-play_animation) ( `animation`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

