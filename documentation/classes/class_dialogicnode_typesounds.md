
<div class="header-banner purple">
<div class="header-label purple">DialogicNode_TypeSounds</div>
</div>

*This contains the source code documentation of the class `DialogicNode_TypeSounds`.*
        
# DialogicNode_TypeSounds
**Inherits:** [AudioStreamPlayer](https://docs.godotengine.org/en/latest/classes/class_audiostreamplayer.html#class-audiostreamplayer)

Node that allows playing sounds when text characters are revealed. Should be the child of a DialogicNode_DialogText node!
## Properties
Name | Type | Default 
--- | --- | --- 
RNG | [RandomNumberGenerator](https://docs.godotengine.org/en/latest/classes/class_randomnumbergenerator.html#class-randomnumbergenerator) |   
base_pitch | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |   
base_volume | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |   
characters_since_last_sound | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
current_overwrite_data | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
enabled | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
end_sound | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
ignore_characters | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `" .,"` 
mode | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
pitch_variance | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
play_every_character | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `1` 
sounds | [AudioStream[]](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
volume_variance | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_overwrite</span>](#property-load_overwrite) ( `dictionary`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">[AudioStream[]](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream)</span> | [<span class="hljs-title">load_sounds_from_path</span>](#property-load_sounds_from_path) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
--- 
## Constants


<a class="header" id="constant-INTERRUPT" href="#constant-INTERRUPT">**<span class="hljs-attribute">const</span> <span class="hljs-title">INTERRUPT</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-OVERLAP" href="#constant-OVERLAP">**<span class="hljs-attribute">const</span> <span class="hljs-title">OVERLAP</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-AWAIT" href="#constant-AWAIT">**<span class="hljs-attribute">const</span> <span class="hljs-title">AWAIT</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-load_overwrite" href="#property-load_overwrite">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_overwrite</span>](#property-load_overwrite) ( `dictionary`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-load_sounds_from_path" href="#property-load_sounds_from_path">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_sounds_from_path</span>](#property-load_sounds_from_path) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[AudioStream[]](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

