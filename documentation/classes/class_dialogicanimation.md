
<div class="header-banner purple">
<div class="header-label purple">DialogicAnimation</div>
</div>

*This contains the source code documentation of the class `DialogicAnimation`.*
        
# DialogicAnimation
**Inherits:** Node

Class that can be used to animate portraits. Can be extended to create animations.
## Properties
Name | Type | Default 
--- | --- | --- 
end_position | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |   
node | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |   
orig_pos | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |   
repeats | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |   
time | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">animate</span>](#property-animate) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">finished_one_loop</span>](#property-finished_one_loop) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">pause</span>](#property-pause) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">resume</span>](#property-resume) ( ) 
--- 

## Signals


<a class="header" id="signal-finished" href="#signal-finished">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">finished</span>](#signal-finished) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-finished_once" href="#signal-finished_once">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">finished_once</span>](#signal-finished_once) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-animate" href="#property-animate">**<span class="hljs-attribute">void</span> [<span class="hljs-title">animate</span>](#property-animate) ( )** </a>



To be overridden. Do the actual animating/tweening in here. Use the properties [node], [time], [end_position], [orig_pos].

---



<a class="header" id="property-finished_one_loop" href="#property-finished_one_loop">**<span class="hljs-attribute">void</span> [<span class="hljs-title">finished_one_loop</span>](#property-finished_one_loop) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-pause" href="#property-pause">**<span class="hljs-attribute">void</span> [<span class="hljs-title">pause</span>](#property-pause) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-resume" href="#property-resume">**<span class="hljs-attribute">void</span> [<span class="hljs-title">resume</span>](#property-resume) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

