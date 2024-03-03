
<div class="header-banner purple">
<div class="header-label purple">DialogicNode_TextBubble</div>
</div>

*This contains the source code documentation of the class `DialogicNode_TextBubble`.*
        
# DialogicNode_TextBubble
**Inherits:** [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)


## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">base_direction</span>](#property-base_direction) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |   
[<span class="hljs-title">base_position</span>](#property-base_position) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |  `Vector2(0, 0)` 
[<span class="hljs-title">bubble_rect</span>](#property-bubble_rect) | [Rect2](https://docs.godotengine.org/en/latest/classes/class_rect2.html#class-rect2) |  `Rect2(0, 0, 2, 2)` 
[<span class="hljs-title">character</span>](#property-character) | [DialogicCharacter](class_dialogiccharacter.md) |  `null` 
[<span class="hljs-title">max_width</span>](#property-max_width) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `300` 
[<span class="hljs-title">padding</span>](#property-padding) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |  `Vector2(0, 0)` 
[<span class="hljs-title">safe_zone</span>](#property-safe_zone) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `50.0` 
[<span class="hljs-title">speaker_node</span>](#property-speaker_node) | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |  `null` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">close</span>](#method-close) ( ) 
<span class="hljs-attribute">[Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)</span> | [<span class="hljs-title">get_bubble</span>](#method-get_bubble) ( ) 
<span class="hljs-attribute">[Container](https://docs.godotengine.org/en/latest/classes/class_container.html#class-container)</span> | [<span class="hljs-title">get_choice_container</span>](#method-get_choice_container) ( ) 
<span class="hljs-attribute">[DialogicNode_DialogText](class_dialogicnode_dialogtext.md)</span> | [<span class="hljs-title">get_dialog_text</span>](#method-get_dialog_text) ( ) 
<span class="hljs-attribute">[DialogicNode_NameLabel](class_dialogicnode_namelabel.md)</span> | [<span class="hljs-title">get_name_label</span>](#method-get_name_label) ( ) 
<span class="hljs-attribute">[PanelContainer](https://docs.godotengine.org/en/latest/classes/class_panelcontainer.html#class-panelcontainer)</span> | [<span class="hljs-title">get_name_label_panel</span>](#method-get_name_label_panel) ( ) 
<span class="hljs-attribute">[Line2D](https://docs.godotengine.org/en/latest/classes/class_line2d.html#class-line2d)</span> | [<span class="hljs-title">get_tail</span>](#method-get_tail) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">open</span>](#method-open) ( ) 
--- 
## Property Descriptions



<a class="header" id="property-base_direction" href="#property-base_direction">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_direction</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-base_position" href="#property-base_position">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_position</span> <span style = "color: gray"> = </span> Vector2(0, 0)** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-bubble_rect" href="#property-bubble_rect">**<span class="hljs-attribute">var</span> <span class="hljs-title">bubble_rect</span> <span style = "color: gray"> = </span> Rect2(0, 0, 2, 2)** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-character" href="#property-character">**<span class="hljs-attribute">var</span> <span class="hljs-title">character</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-max_width" href="#property-max_width">**<span class="hljs-attribute">var</span> <span class="hljs-title">max_width</span> <span style = "color: gray"> = </span> 300** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-padding" href="#property-padding">**<span class="hljs-attribute">var</span> <span class="hljs-title">padding</span> <span style = "color: gray"> = </span> Vector2(0, 0)** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-safe_zone" href="#property-safe_zone">**<span class="hljs-attribute">var</span> <span class="hljs-title">safe_zone</span> <span style = "color: gray"> = </span> 50.0** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-speaker_node" href="#property-speaker_node">**<span class="hljs-attribute">var</span> <span class="hljs-title">speaker_node</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-close" href="#method-close">**<span class="hljs-attribute">func</span> [<span class="hljs-title">close</span>](#method-close) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_bubble" href="#method-get_bubble">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_bubble</span>](#method-get_bubble) ( )</a>  ⇒ <span class="hljs-attribute">[Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_choice_container" href="#method-get_choice_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_choice_container</span>](#method-get_choice_container) ( )</a>  ⇒ <span class="hljs-attribute">[Container](https://docs.godotengine.org/en/latest/classes/class_container.html#class-container)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_dialog_text" href="#method-get_dialog_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_dialog_text</span>](#method-get_dialog_text) ( )</a>  ⇒ <span class="hljs-attribute">[DialogicNode_DialogText](class_dialogicnode_dialogtext.md)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_name_label" href="#method-get_name_label">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_name_label</span>](#method-get_name_label) ( )</a>  ⇒ <span class="hljs-attribute">[DialogicNode_NameLabel](class_dialogicnode_namelabel.md)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_name_label_panel" href="#method-get_name_label_panel">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_name_label_panel</span>](#method-get_name_label_panel) ( )</a>  ⇒ <span class="hljs-attribute">[PanelContainer](https://docs.godotengine.org/en/latest/classes/class_panelcontainer.html#class-panelcontainer)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_tail" href="#method-get_tail">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_tail</span>](#method-get_tail) ( )</a>  ⇒ <span class="hljs-attribute">[Line2D](https://docs.godotengine.org/en/latest/classes/class_line2d.html#class-line2d)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-open" href="#method-open">**<span class="hljs-attribute">func</span> [<span class="hljs-title">open</span>](#method-open) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

