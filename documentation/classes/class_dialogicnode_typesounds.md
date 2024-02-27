
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
[<span class="hljs-title">RNG</span>](#property-rng) | [RandomNumberGenerator](https://docs.godotengine.org/en/latest/classes/class_randomnumbergenerator.html#class-randomnumbergenerator) |   
[<span class="hljs-title">base_pitch</span>](#property-base_pitch) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |   
[<span class="hljs-title">base_volume</span>](#property-base_volume) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |   
[<span class="hljs-title">characters_since_last_sound</span>](#property-characters_since_last_sound) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">current_overwrite_data</span>](#property-current_overwrite_data) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">enabled</span>](#property-enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">end_sound</span>](#property-end_sound) | [AudioStream](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
[<span class="hljs-title">ignore_characters</span>](#property-ignore_characters) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `" .,"` 
[<span class="hljs-title">mode</span>](#property-mode) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">pitch_variance</span>](#property-pitch_variance) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
[<span class="hljs-title">play_every_character</span>](#property-play_every_character) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `1` 
[<span class="hljs-title">sounds</span>](#property-sounds) | [AudioStream[]](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream) |   
[<span class="hljs-title">volume_variance</span>](#property-volume_variance) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
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



<a class="header" id="property-rng" href="#property-rng">**<span class="hljs-attribute">var</span> <span class="hljs-title">RNG</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-base_pitch" href="#property-base_pitch">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_pitch</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-base_volume" href="#property-base_volume">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_volume</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-characters_since_last_sound" href="#property-characters_since_last_sound">**<span class="hljs-attribute">var</span> <span class="hljs-title">characters_since_last_sound</span> <span style = "color: gray"> = </span> 0** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-current_overwrite_data" href="#property-current_overwrite_data">**<span class="hljs-attribute">var</span> <span class="hljs-title">current_overwrite_data</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-enabled" href="#property-enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">enabled</span> <span style = "color: gray"> = </span> true** 



Usefull if you want to change the sounds of different node's sounds

---



<a class="header" id="property-end_sound" href="#property-end_sound">**<span class="hljs-attribute">var</span> <span class="hljs-title">end_sound</span>** 



A sound to be played as the last sound.

---



<a class="header" id="property-ignore_characters" href="#property-ignore_characters">**<span class="hljs-attribute">var</span> <span class="hljs-title">ignore_characters</span> <span style = "color: gray"> = </span> " .,"** 



Characters that don't increase the 'characters_since_last_sound' variable, useful for the space or fullstop

---



<a class="header" id="property-mode" href="#property-mode">**<span class="hljs-attribute">var</span> <span class="hljs-title">mode</span> <span style = "color: gray"> = </span> 0** 



If true, interrupts the current sound to play a new one

---



<a class="header" id="property-pitch_variance" href="#property-pitch_variance">**<span class="hljs-attribute">var</span> <span class="hljs-title">pitch_variance</span> <span style = "color: gray"> = </span> 0.0** 



Allows changing the pitch by a random value from (pitch - pitch_variance) to (pitch + pitch_variance)

---



<a class="header" id="property-play_every_character" href="#property-play_every_character">**<span class="hljs-attribute">var</span> <span class="hljs-title">play_every_character</span> <span style = "color: gray"> = </span> 1** 



Determines how many characters are between each sound. Default is 1 for playing it every character.

---



<a class="header" id="property-sounds" href="#property-sounds">**<span class="hljs-attribute">var</span> <span class="hljs-title">sounds</span> <span style = "color: gray"> = </span> <unknown>** 



Array of sounds. Will pick a random one each time.

---



<a class="header" id="property-volume_variance" href="#property-volume_variance">**<span class="hljs-attribute">var</span> <span class="hljs-title">volume_variance</span> <span style = "color: gray"> = </span> 0.0** 



Allows changing the volume by a random value from (volume - volume_variance) to (volume + volume_variance)

---

## Methods Descriptions



<a class="header" id="method-load_overwrite" href="#method-load_overwrite">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_overwrite</span>](#property-load_overwrite) ( `dictionary`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-load_sounds_from_path" href="#method-load_sounds_from_path">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_sounds_from_path</span>](#property-load_sounds_from_path) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[AudioStream[]](https://docs.godotengine.org/en/latest/classes/class_audiostream.html#class-audiostream)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

