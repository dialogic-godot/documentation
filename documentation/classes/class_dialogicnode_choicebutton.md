
<div class="header-banner purple">
<div class="header-label purple">DialogicNode_ChoiceButton</div>
</div>

*This contains the source code documentation of the class `DialogicNode_ChoiceButton`.*
        
# DialogicNode_ChoiceButton
**Inherits:** [Button](https://docs.godotengine.org/en/latest/classes/class_button.html#class-button)

The button allows the player to make a choice in the Dialogic system.
## Description
This class is used in the Choice Layer. 
You may change the `text_node` to any [Node](class_node.md) that has a `text` property. 
If you don't set the `text_node`, the text will be set on this button instead.  Using a different node may allow using rich text effects; they are not supported on buttons at this point.

## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">choice_index</span>](#property-choice_index) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `-1` 
[<span class="hljs-title">sound_focus</span>](#property-sound_focus) | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
[<span class="hljs-title">sound_hover</span>](#property-sound_hover) | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
[<span class="hljs-title">sound_pressed</span>](#property-sound_pressed) | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
[<span class="hljs-title">text_node</span>](#property-text_node) | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |   
## Property Descriptions



<a class="header" id="property-choice_index" href="#property-choice_index">**<span class="hljs-attribute">var</span> <span class="hljs-title">choice_index</span> <span style = "color: gray"> = </span> -1** 



Used to identify what choices to put on. If you leave it at -1, choices will be distributed automatically.

---



<a class="header" id="property-sound_focus" href="#property-sound_focus">**<span class="hljs-attribute">var</span> <span class="hljs-title">sound_focus</span>** 



Can be set to play this sound when focused. Requires a sibling DialogicNode_ButtonSound node.

---



<a class="header" id="property-sound_hover" href="#property-sound_hover">**<span class="hljs-attribute">var</span> <span class="hljs-title">sound_hover</span>** 



Can be set to play this sound when hovered. Requires a sibling DialogicNode_ButtonSound node.

---



<a class="header" id="property-sound_pressed" href="#property-sound_pressed">**<span class="hljs-attribute">var</span> <span class="hljs-title">sound_pressed</span>** 



Can be set to play this sound when pressed. Requires a sibling DialogicNode_ButtonSound node.

---



<a class="header" id="property-text_node" href="#property-text_node">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_node</span>** 



If set, the text will be set on this node's `text` property instead.

---

