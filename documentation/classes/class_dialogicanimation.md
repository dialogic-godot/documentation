
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
[<span class="hljs-title">end_position</span>](#property-end_position) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |   
[<span class="hljs-title">node</span>](#property-node) | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |   
[<span class="hljs-title">orig_pos</span>](#property-orig_pos) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |   
[<span class="hljs-title">repeats</span>](#property-repeats) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |   
[<span class="hljs-title">time</span>](#property-time) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">animate</span>](#property-animate) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">finished_one_loop</span>](#property-finished_one_loop) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">pause</span>](#property-pause) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume</span>](#property-resume) ( ) 
--- 

## Signals


<a class="header" id="signal-finished" href="#signal-finished">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">finished</span>](#signal-finished) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-finished_once" href="#signal-finished_once">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">finished_once</span>](#signal-finished_once) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-end_position" href="#property-end_position">**<span class="hljs-attribute">var</span> <span class="hljs-title">end_position</span>** 



Set at runtime, will be the position at which to end the animation.

---



<a class="header" id="property-node" href="#property-node">**<span class="hljs-attribute">var</span> <span class="hljs-title">node</span>** 



Set at runtime, will be the node to animate.

---



<a class="header" id="property-orig_pos" href="#property-orig_pos">**<span class="hljs-attribute">var</span> <span class="hljs-title">orig_pos</span>** 



Set at runtime. The position the node started at.

---



<a class="header" id="property-repeats" href="#property-repeats">**<span class="hljs-attribute">var</span> <span class="hljs-title">repeats</span>** 



Used to repeate the animation for a number of times.

---



<a class="header" id="property-time" href="#property-time">**<span class="hljs-attribute">var</span> <span class="hljs-title">time</span>** 



Set at runtime, will be the length of the animation.

---

## Methods Descriptions



<a class="header" id="method-animate" href="#method-animate">**<span class="hljs-attribute">func</span> [<span class="hljs-title">animate</span>](#property-animate) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



To be overridden. Do the actual animating/tweening in here. Use the properties [node], [time], [end_position], [orig_pos].

---



<a class="header" id="method-finished_one_loop" href="#method-finished_one_loop">**<span class="hljs-attribute">func</span> [<span class="hljs-title">finished_one_loop</span>](#property-finished_one_loop) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-pause" href="#method-pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pause</span>](#property-pause) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-resume" href="#method-resume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume</span>](#property-resume) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

