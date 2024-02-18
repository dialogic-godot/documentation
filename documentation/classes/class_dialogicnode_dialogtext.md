
<div class="header-banner purple">
<div class="header-label purple">DialogicNode_DialogText</div>
</div>

*This contains the source code documentation of the class `DialogicNode_DialogText`.*
        
# DialogicNode_DialogText
**Inherits:** [RichTextLabel](https://docs.godotengine.org/en/latest/classes/class_richtextlabel.html#class-richtextlabel)

Dialogic node that can reveal text at a given (changeable speed).
## Properties
Name | Type | Default 
--- | --- | --- 
active_speed | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.01` 
alignment | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
base_visible_characters | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
enabled | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
hide_when_empty | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
revealing | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
speed_counter | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
start_hidden | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
textbox_root | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">continue_reveal</span>](#property-continue_reveal) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">finish_text</span>](#property-finish_text) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reveal_text</span>](#property-reveal_text) ( `_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `keep_previous`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_speed</span>](#property-set_speed) ( `delay_per_character`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) ) 
--- 
## Constants


<a class="header" id="constant-LEFT" href="#constant-LEFT">**<span class="hljs-attribute">const</span> <span class="hljs-title">LEFT</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-CENTER" href="#constant-CENTER">**<span class="hljs-attribute">const</span> <span class="hljs-title">CENTER</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-RIGHT" href="#constant-RIGHT">**<span class="hljs-attribute">const</span> <span class="hljs-title">RIGHT</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-continued_revealing_text" href="#signal-continued_revealing_text">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">continued_revealing_text</span>](#signal-continued_revealing_text) ( `new_character`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-finished_revealing_text" href="#signal-finished_revealing_text">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">finished_revealing_text</span>](#signal-finished_revealing_text) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-started_revealing_text" href="#signal-started_revealing_text">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">started_revealing_text</span>](#signal-started_revealing_text) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-continue_reveal" href="#property-continue_reveal">**<span class="hljs-attribute">func</span> [<span class="hljs-title">continue_reveal</span>](#property-continue_reveal) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Reveals one additional character.

---



<a class="header" id="property-finish_text" href="#property-finish_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">finish_text</span>](#property-finish_text) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Reveals the entire text instantly.

---



<a class="header" id="property-reveal_text" href="#property-reveal_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reveal_text</span>](#property-reveal_text) ( `_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `keep_previous`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_speed" href="#property-set_speed">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_speed</span>](#property-set_speed) ( `delay_per_character`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

