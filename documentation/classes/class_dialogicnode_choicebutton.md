
<div class="header-banner purple">
<div class="header-label purple">DialogicNode_ChoiceButton</div>
</div>

*This contains the source code documentation of the class `DialogicNode_ChoiceButton`.*
        
# DialogicNode_ChoiceButton
**Inherits:** [Button](https://docs.godotengine.org/en/latest/classes/class_button.html#class-button)

This button allows the player to make a choice in the Dialogic system.
## Description
When a choice is reached Dialogic will automatically show ChoiceButtons and call their _load_info()[/code] method which will display the choices. You will need to ensure that enough choice buttons are available in the tree to display all choices.

You can extend this node and implement some custom logic by overwriting the _load_info(info:Dictionary)[/code] method. 

If you need RichText support, consider adding a RichTextLabel child and setting it as the `text_node`.

DialogicChoiceButtons will grab the focus when hovered to avoid a confusing focus style being present for players who use the mouse.
To avoid the opposite situation, when the focus is changed by the player and a different button is still hovered the mouse pointer will be moved to the now focused button as well.

## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">choice_index</span>](#property-choice_index) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `-1` 
[<span class="hljs-title">sound_pressed</span>](#property-sound_pressed) | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
[<span class="hljs-title">sound_hover</span>](#property-sound_hover) | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
[<span class="hljs-title">sound_focus</span>](#property-sound_focus) | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
[<span class="hljs-title">text_node</span>](#property-text_node) | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_choice_text</span>](#method-set_choice_text) ( `new_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
--- 

## Signals


<a class="header" id="signal-choice_selected" href="#signal-choice_selected">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">choice_selected</span>](#signal-choice_selected) ( )** </a>



 Emitted when the choice is selected. Unless overridden, this is when the button or its shortcut is pressed. 

---

## Property Descriptions



<a class="header" id="property-choice_index" href="#property-choice_index">**<span class="hljs-attribute">var</span> <span class="hljs-title">choice_index</span> <span style = "color: gray"> = </span> -1** 



Used to identify what choices to put on. If you leave it at -1, choices will be distributed automatically.

---



<a class="header" id="property-sound_pressed" href="#property-sound_pressed">**<span class="hljs-attribute">var</span> <span class="hljs-title">sound_pressed</span>** 



Can be set to play this sound when pressed. Requires a sibling DialogicNode_ButtonSound node.

---



<a class="header" id="property-sound_hover" href="#property-sound_hover">**<span class="hljs-attribute">var</span> <span class="hljs-title">sound_hover</span>** 



Can be set to play this sound when hovered. Requires a sibling DialogicNode_ButtonSound node.

---



<a class="header" id="property-sound_focus" href="#property-sound_focus">**<span class="hljs-attribute">var</span> <span class="hljs-title">sound_focus</span>** 



Can be set to play this sound when focused. Requires a sibling DialogicNode_ButtonSound node.

---



<a class="header" id="property-text_node" href="#property-text_node">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_node</span>** 



If set, the text will be set on this node's `text` property instead. This can be used to have a custom text rendering child, like a RichTextLabel.

---

## Method Descriptions



<a class="header" id="method-set_choice_text" href="#method-set_choice_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_choice_text</span>](#method-set_choice_text) ( `new_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Called when the text changes.

---

