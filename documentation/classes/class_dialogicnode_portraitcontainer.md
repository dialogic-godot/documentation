
<div class="header-banner purple">
<div class="header-label purple">DialogicNode_PortraitContainer</div>
</div>

*This contains the source code documentation of the class `DialogicNode_PortraitContainer`.*
        
# DialogicNode_PortraitContainer
**Inherits:** [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)

Node that defines a position for dialogic portraits and how to display portrait at that position.
## Properties
Name | Type | Default 
--- | --- | --- 
debug_character | [DialogicCharacter](class_dialogiccharacter.md) |  `null` 
debug_character_holder_node | [Node2D](https://docs.godotengine.org/en/latest/classes/class_node2d.html#class-node2d) |  `null` 
debug_character_portrait | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
debug_character_scene_node | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |  `null` 
debug_origin | [Sprite2D](https://docs.godotengine.org/en/latest/classes/class_sprite2d.html#class-sprite2d) |  `null` 
default_debug_character | [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource) |   
default_portrait_scene | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
mirrored | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
mode | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
origin_anchor | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `7` 
origin_offset | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |  `Vector2(0, 0)` 
portrait_prefix | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
position_index | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
size_mode | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `3` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[Rect2](https://docs.godotengine.org/en/latest/classes/class_rect2.html#class-rect2)</span> | [<span class="hljs-title">get_local_portrait_transform</span>](#property-get_local_portrait_transform) ( `portrait_rect`: [Rect2](https://docs.godotengine.org/en/latest/classes/class_rect2.html#class-rect2), `character_scale`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_portrait_transforms</span>](#property-update_portrait_transforms) ( ) 
--- 
## Constants


<a class="header" id="constant-POSITION" href="#constant-POSITION">**<span class="hljs-attribute">const</span> <span class="hljs-title">POSITION</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-SPEAKER" href="#constant-SPEAKER">**<span class="hljs-attribute">const</span> <span class="hljs-title">SPEAKER</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-KEEP" href="#constant-KEEP">**<span class="hljs-attribute">const</span> <span class="hljs-title">KEEP</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-FIT_STRETCH" href="#constant-FIT_STRETCH">**<span class="hljs-attribute">const</span> <span class="hljs-title">FIT_STRETCH</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-FIT_IGNORE_SCALE" href="#constant-FIT_IGNORE_SCALE">**<span class="hljs-attribute">const</span> <span class="hljs-title">FIT_IGNORE_SCALE</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-FIT_SCALE_HEIGHT" href="#constant-FIT_SCALE_HEIGHT">**<span class="hljs-attribute">const</span> <span class="hljs-title">FIT_SCALE_HEIGHT</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TOP_LEFT" href="#constant-TOP_LEFT">**<span class="hljs-attribute">const</span> <span class="hljs-title">TOP_LEFT</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TOP_CENTER" href="#constant-TOP_CENTER">**<span class="hljs-attribute">const</span> <span class="hljs-title">TOP_CENTER</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TOP_RIGHT" href="#constant-TOP_RIGHT">**<span class="hljs-attribute">const</span> <span class="hljs-title">TOP_RIGHT</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-LEFT_MIDDLE" href="#constant-LEFT_MIDDLE">**<span class="hljs-attribute">const</span> <span class="hljs-title">LEFT_MIDDLE</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-CENTER" href="#constant-CENTER">**<span class="hljs-attribute">const</span> <span class="hljs-title">CENTER</span><span class="hljs-comment"> = 4</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-RIGHT_MIDDLE" href="#constant-RIGHT_MIDDLE">**<span class="hljs-attribute">const</span> <span class="hljs-title">RIGHT_MIDDLE</span><span class="hljs-comment"> = 5</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-BOTTOM_LEFT" href="#constant-BOTTOM_LEFT">**<span class="hljs-attribute">const</span> <span class="hljs-title">BOTTOM_LEFT</span><span class="hljs-comment"> = 6</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-BOTTOM_CENTER" href="#constant-BOTTOM_CENTER">**<span class="hljs-attribute">const</span> <span class="hljs-title">BOTTOM_CENTER</span><span class="hljs-comment"> = 7</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-BOTTOM_RIGHT" href="#constant-BOTTOM_RIGHT">**<span class="hljs-attribute">const</span> <span class="hljs-title">BOTTOM_RIGHT</span><span class="hljs-comment"> = 8</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-get_local_portrait_transform" href="#property-get_local_portrait_transform">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_local_portrait_transform</span>](#property-get_local_portrait_transform) ( `portrait_rect`: [Rect2](https://docs.godotengine.org/en/latest/classes/class_rect2.html#class-rect2), `character_scale`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` )</a>  ⇒ <span class="hljs-attribute">[Rect2](https://docs.godotengine.org/en/latest/classes/class_rect2.html#class-rect2)</span>** 



Returns a Rect2 with the position as the position and the scale as the size.

---



<a class="header" id="property-update_portrait_transforms" href="#property-update_portrait_transforms">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_portrait_transforms</span>](#property-update_portrait_transforms) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

