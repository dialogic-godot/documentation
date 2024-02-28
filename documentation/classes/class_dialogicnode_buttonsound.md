
<div class="header-banner purple">
<div class="header-label purple">DialogicNode_ButtonSound</div>
</div>

*This contains the source code documentation of the class `DialogicNode_ButtonSound`.*
        
# DialogicNode_ButtonSound
**Inherits:** [AudioStreamPlayer](https://docs.godotengine.org/en/latest/classes/class_audiostreamplayer.html#class-audiostreamplayer)

Node that is used for playing sound effects on hover/focus/press of sibling DialogicNode_ChoiceButtons.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">sound_focus</span>](#property-sound_focus) | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
[<span class="hljs-title">sound_hover</span>](#property-sound_hover) | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
[<span class="hljs-title">sound_pressed</span>](#property-sound_pressed) | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">play_sound</span>](#property-play_sound) ( `sound`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
--- 
## Property Descriptions



<a class="header" id="property-sound_focus" href="#property-sound_focus">**<span class="hljs-attribute">var</span> <span class="hljs-title">sound_focus</span>** 



Sound to be played on focus. See [sound_pressed] for more.

---



<a class="header" id="property-sound_hover" href="#property-sound_hover">**<span class="hljs-attribute">var</span> <span class="hljs-title">sound_hover</span>** 



Sound to be played on hover. See [sound_pressed] for more.

---



<a class="header" id="property-sound_pressed" href="#property-sound_pressed">**<span class="hljs-attribute">var</span> <span class="hljs-title">sound_pressed</span>** 



Sound to be played if one of the sibling ChoiceButtons is pressed. If sibling ChoiceButton has a sound_pressed set, that is prioritized.

---

## Method Descriptions



<a class="header" id="method-play_sound" href="#method-play_sound">**<span class="hljs-attribute">func</span> [<span class="hljs-title">play_sound</span>](#property-play_sound) ( `sound`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

