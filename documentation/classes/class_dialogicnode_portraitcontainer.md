
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
[<span class="hljs-title">debug_character</span>](#property-debug_character) | [DialogicCharacter](class_dialogiccharacter.md) |  `null` 
[<span class="hljs-title">debug_character_holder_node</span>](#property-debug_character_holder_node) | [Node2D](https://docs.godotengine.org/en/latest/classes/class_node2d.html#class-node2d) |  `null` 
[<span class="hljs-title">debug_character_portrait</span>](#property-debug_character_portrait) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">debug_character_scene_node</span>](#property-debug_character_scene_node) | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |  `null` 
[<span class="hljs-title">debug_origin</span>](#property-debug_origin) | [Sprite2D](https://docs.godotengine.org/en/latest/classes/class_sprite2d.html#class-sprite2d) |  `null` 
[<span class="hljs-title">default_debug_character</span>](#property-default_debug_character) | [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource) |   
[<span class="hljs-title">default_portrait_scene</span>](#property-default_portrait_scene) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
[<span class="hljs-title">mirrored</span>](#property-mirrored) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">mode</span>](#property-mode) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">origin_anchor</span>](#property-origin_anchor) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `7` 
[<span class="hljs-title">origin_offset</span>](#property-origin_offset) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |  `Vector2(0, 0)` 
[<span class="hljs-title">portrait_prefix</span>](#property-portrait_prefix) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">position_index</span>](#property-position_index) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">size_mode</span>](#property-size_mode) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `3` 
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



<a class="header" id="property-debug_character" href="#property-debug_character">**<span class="hljs-attribute">var</span> <span class="hljs-title">debug_character</span> <span style = "color: gray"> = </span> null** 



A character that will be displayed in the editor, useful for getting the right size.

---



<a class="header" id="property-debug_character_holder_node" href="#property-debug_character_holder_node">**<span class="hljs-attribute">var</span> <span class="hljs-title">debug_character_holder_node</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-debug_character_portrait" href="#property-debug_character_portrait">**<span class="hljs-attribute">var</span> <span class="hljs-title">debug_character_portrait</span> <span style = "color: gray"> = </span> ""** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-debug_character_scene_node" href="#property-debug_character_scene_node">**<span class="hljs-attribute">var</span> <span class="hljs-title">debug_character_scene_node</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-debug_origin" href="#property-debug_origin">**<span class="hljs-attribute">var</span> <span class="hljs-title">debug_origin</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-default_debug_character" href="#property-default_debug_character">**<span class="hljs-attribute">var</span> <span class="hljs-title">default_debug_character</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-default_portrait_scene" href="#property-default_portrait_scene">**<span class="hljs-attribute">var</span> <span class="hljs-title">default_portrait_scene</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-mirrored" href="#property-mirrored">**<span class="hljs-attribute">var</span> <span class="hljs-title">mirrored</span> <span style = "color: gray"> = </span> false** 



If true, portraits will be mirrored in this position.

---



<a class="header" id="property-mode" href="#property-mode">**<span class="hljs-attribute">var</span> <span class="hljs-title">mode</span> <span style = "color: gray"> = </span> 0** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-origin_anchor" href="#property-origin_anchor">**<span class="hljs-attribute">var</span> <span class="hljs-title">origin_anchor</span> <span style = "color: gray"> = </span> 7** 



The portrait will be placed relative to this point in the container.

---



<a class="header" id="property-origin_offset" href="#property-origin_offset">**<span class="hljs-attribute">var</span> <span class="hljs-title">origin_offset</span> <span style = "color: gray"> = </span> Vector2(0, 0)** 



An offset to apply to the origin. Rarely useful.

---



<a class="header" id="property-portrait_prefix" href="#property-portrait_prefix">**<span class="hljs-attribute">var</span> <span class="hljs-title">portrait_prefix</span> <span style = "color: gray"> = </span> ""** 



Can be used to use a different portrait. E.g. "Faces/" would mean instead of "happy" it will use portrait "Faces/happy"

---



<a class="header" id="property-position_index" href="#property-position_index">**<span class="hljs-attribute">var</span> <span class="hljs-title">position_index</span> <span style = "color: gray"> = </span> 0** 



The position this node corresponds to.

---



<a class="header" id="property-size_mode" href="#property-size_mode">**<span class="hljs-attribute">var</span> <span class="hljs-title">size_mode</span> <span style = "color: gray"> = </span> 3** 



Defines how to affect the scale of the portrait

---

## Method Descriptions



<a class="header" id="method-get_local_portrait_transform" href="#method-get_local_portrait_transform">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_local_portrait_transform</span>](#property-get_local_portrait_transform) ( `portrait_rect`: [Rect2](https://docs.godotengine.org/en/latest/classes/class_rect2.html#class-rect2), `character_scale`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` )</a>  ⇒ <span class="hljs-attribute">[Rect2](https://docs.godotengine.org/en/latest/classes/class_rect2.html#class-rect2)</span>** 



Returns a Rect2 with the position as the position and the scale as the size.

---



<a class="header" id="method-update_portrait_transforms" href="#method-update_portrait_transforms">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_portrait_transforms</span>](#property-update_portrait_transforms) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

