
<div class="header-banner purple">
<div class="header-label purple">DialogicAnimation</div>
</div>

*This contains the source code documentation of the class `DialogicAnimation`.*
        
# DialogicAnimation
**Inherits:** [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)

Class that can be used to animate portraits. Can be extended to create animations.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">node</span>](#property-node) | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |   
[<span class="hljs-title">time</span>](#property-time) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |   
[<span class="hljs-title">base_position</span>](#property-base_position) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |   
[<span class="hljs-title">base_scale</span>](#property-base_scale) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |   
[<span class="hljs-title">repeats</span>](#property-repeats) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |   
[<span class="hljs-title">is_reversed</span>](#property-is_reversed) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">animate</span>](#method-animate) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">finished_one_loop</span>](#method-finished_one_loop) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">pause</span>](#method-pause) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume</span>](#method-resume) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_modulation_property</span>](#method-get_modulation_property) ( ) 
<span class="hljs-attribute">[Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2)</span> | [<span class="hljs-title">get_node_size</span>](#method-get_node_size) ( ) 
<span class="hljs-attribute">[Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2)</span> | [<span class="hljs-title">get_node_origin</span>](#method-get_node_origin) ( ) 
<span class="hljs-attribute">[Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2)</span> | [<span class="hljs-title">get_viewport_size</span>](#method-get_viewport_size) ( ) 
--- 
## Constants


<a class="header" id="constant-IN" href="#constant-IN">**<span class="hljs-attribute">const</span> <span class="hljs-title">IN</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-OUT" href="#constant-OUT">**<span class="hljs-attribute">const</span> <span class="hljs-title">OUT</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ACTION" href="#constant-ACTION">**<span class="hljs-attribute">const</span> <span class="hljs-title">ACTION</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-CROSSFADE" href="#constant-CROSSFADE">**<span class="hljs-attribute">const</span> <span class="hljs-title">CROSSFADE</span><span class="hljs-comment"> = 4</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-finished_once" href="#signal-finished_once">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">finished_once</span>](#signal-finished_once) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-finished" href="#signal-finished">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">finished</span>](#signal-finished) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-node" href="#property-node">**<span class="hljs-attribute">var</span> <span class="hljs-title">node</span>** 



Set at runtime, will be the node to animate.

---



<a class="header" id="property-time" href="#property-time">**<span class="hljs-attribute">var</span> <span class="hljs-title">time</span>** 



Set at runtime, will be the length of the animation.

---



<a class="header" id="property-base_position" href="#property-base_position">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_position</span>** 



Set at runtime, will be the base position of the node. Depending on the animation, this might be the start, end or both.

---



<a class="header" id="property-base_scale" href="#property-base_scale">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_scale</span>** 



Set at runtime, will be the base scale of the node.

---



<a class="header" id="property-repeats" href="#property-repeats">**<span class="hljs-attribute">var</span> <span class="hljs-title">repeats</span>** 



Used to repeate the animation for a number of times.

---



<a class="header" id="property-is_reversed" href="#property-is_reversed">**<span class="hljs-attribute">var</span> <span class="hljs-title">is_reversed</span> <span style = "color: gray"> = </span> false** 



If `true`, the animation will be reversed. This must be implemented by each animation or it will have no effect.

---

## Method Descriptions



<a class="header" id="method-animate" href="#method-animate">**<span class="hljs-attribute">func</span> [<span class="hljs-title">animate</span>](#method-animate) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



To be overridden. Do the actual animating/tweening in here. Use the properties `node`, `time`, `base_position`, etc.

---



<a class="header" id="method-finished_one_loop" href="#method-finished_one_loop">**<span class="hljs-attribute">func</span> [<span class="hljs-title">finished_one_loop</span>](#method-finished_one_loop) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



This method controls whether to repeat the animation or not. Animations must call this once they finished an animation.

---



<a class="header" id="method-pause" href="#method-pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pause</span>](#method-pause) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-resume" href="#method-resume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume</span>](#method-resume) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_modulation_property" href="#method-get_modulation_property">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_modulation_property</span>](#method-get_modulation_property) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



If the animation wants to change the modulation, this method will return the property to change.  The [CanvasGroup](class_canvasgroup.md) can use `self_modulate` instead of `modulate` to uniformly change the modulation of all children without additively overlaying the modulations.

---



<a class="header" id="method-get_node_size" href="#method-get_node_size">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_node_size</span>](#method-get_node_size) ( )</a>  ⇒ <span class="hljs-attribute">[Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2)</span>** 



Tries to return the size of the node to be animated. For portraits this uses the portrait containers size. This is useful if your animation depends on the size of the node.

---



<a class="header" id="method-get_node_origin" href="#method-get_node_origin">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_node_origin</span>](#method-get_node_origin) ( )</a>  ⇒ <span class="hljs-attribute">[Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_viewport_size" href="#method-get_viewport_size">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_viewport_size</span>](#method-get_viewport_size) ( )</a>  ⇒ <span class="hljs-attribute">[Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

