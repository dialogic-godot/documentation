
<div class="header-banner purple">
<div class="header-label purple">Containers</div>
</div>

*This contains the source code documentation of the class `subsystem_Containers`.*
        
# subsystem_Containers
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that manages portrait positions.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">transform_regex</span>](#property-transform_regex) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"(?<part>position|pos|size|siz|rotation|rot)\\W*=(?<value>((?!(pos|siz|rot)).)*)"` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md)</span> | [<span class="hljs-title">get_container</span>](#method-get_container) ( `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[DialogicNode_PortraitContainer[]](https://docs.godotengine.org/en/latest/classes/class_dialogicnode_portraitcontainer.html#class-dialogicnode_portraitcontainer)</span> | [<span class="hljs-title">get_containers</span>](#method-get_containers) ( `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[CanvasItem](https://docs.godotengine.org/en/latest/classes/class_canvasitem.html#class-canvasitem)</span> | [<span class="hljs-title">get_container_container</span>](#method-get_container_container) ( ) 
<span class="hljs-attribute">[DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md)</span> | [<span class="hljs-title">add_container</span>](#method-add_container) ( `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">move_container</span>](#method-move_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `destination`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null`, `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">copy_container_setup</span>](#method-copy_container_setup) ( `from`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `to`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">translate_container</span>](#method-translate_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `translation`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `relative`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null`, `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">rotate_container</span>](#method-rotate_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `rotation`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float), `relative`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null`, `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resize_container</span>](#method-resize_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `rect_size`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `relative`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null`, `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">save_position_container</span>](#method-save_position_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md) ) 
<span class="hljs-attribute">[DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md)</span> | [<span class="hljs-title">load_position_container</span>](#method-load_position_container) ( `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2)</span> | [<span class="hljs-title">str_to_vector</span>](#method-str_to_vector) ( `input`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `base_vector`: [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) = `Vector2(0, 0)` ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">vector_to_str</span>](#method-vector_to_str) ( `vec`: [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset_all_containers</span>](#method-reset_all_containers) ( `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset_container</span>](#method-reset_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null` ) 
--- 

## Signals


<a class="header" id="signal-position_changed" href="#signal-position_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">position_changed</span>](#signal-position_changed) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-transform_regex" href="#property-transform_regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">transform_regex</span> <span style = "color: gray"> = </span> "(?<part>position|pos|size|siz|rotation|rot)\\W*=(?<value>((?!(pos|siz|rot)).)*)"** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-get_container" href="#method-get_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_container</span>](#method-get_container) ( `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_containers" href="#method-get_containers">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_containers</span>](#method-get_containers) ( `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[DialogicNode_PortraitContainer[]](https://docs.godotengine.org/en/latest/classes/class_dialogicnode_portraitcontainer.html#class-dialogicnode_portraitcontainer)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_container_container" href="#method-get_container_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_container_container</span>](#method-get_container_container) ( )</a>  ⇒ <span class="hljs-attribute">[CanvasItem](https://docs.godotengine.org/en/latest/classes/class_canvasitem.html#class-canvasitem)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-add_container" href="#method-add_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_container</span>](#method-add_container) ( `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md)</span>** 



Creates a new portrait container node. It will copy it's size and most settings from the first p_container in the tree. It will be added as a sibling of the first p_container in the tree.

---



<a class="header" id="method-move_container" href="#method-move_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">move_container</span>](#method-move_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `destination`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null`, `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Moves the  to the  (using  and ). The destination can be a position_id (e.g. "center") or translation, roataion and scale. When moving to a preset container, then some more will be "copied" (e.g. anchors, etc.)

---



<a class="header" id="method-copy_container_setup" href="#method-copy_container_setup">**<span class="hljs-attribute">func</span> [<span class="hljs-title">copy_container_setup</span>](#method-copy_container_setup) ( `from`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `to`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-translate_container" href="#method-translate_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">translate_container</span>](#method-translate_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `translation`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `relative`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null`, `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Translates the given container. The given translation should be the target position of the ORIGIN point, not the container!

---



<a class="header" id="method-rotate_container" href="#method-rotate_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">rotate_container</span>](#method-rotate_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `rotation`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float), `relative`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null`, `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-resize_container" href="#method-resize_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resize_container</span>](#method-resize_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `rect_size`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `relative`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null`, `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `1.0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-save_position_container" href="#method-save_position_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">save_position_container</span>](#method-save_position_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-load_position_container" href="#method-load_position_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_position_container</span>](#method-load_position_container) ( `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-str_to_vector" href="#method-str_to_vector">**<span class="hljs-attribute">func</span> [<span class="hljs-title">str_to_vector</span>](#method-str_to_vector) ( `input`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `base_vector`: [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) = `Vector2(0, 0)` )</a>  ⇒ <span class="hljs-attribute">[Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-vector_to_str" href="#method-vector_to_str">**<span class="hljs-attribute">func</span> [<span class="hljs-title">vector_to_str</span>](#method-vector_to_str) ( `vec`: [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-reset_all_containers" href="#method-reset_all_containers">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset_all_containers</span>](#method-reset_all_containers) ( `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-reset_container" href="#method-reset_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset_container</span>](#method-reset_container) ( `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `tween`: [Tween](https://docs.godotengine.org/en/latest/classes/class_tween.html#class-tween) = `null` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

