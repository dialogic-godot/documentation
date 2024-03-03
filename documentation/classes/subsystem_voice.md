
<div class="header-banner purple">
<div class="header-label purple">subsystem_Voice</div>
</div>

*This contains the source code documentation of the class `subsystem_Voice`.*
        
# subsystem_Voice
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

##################################################################################################
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">current_audio_file</span>](#property-current_audio_file) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
[<span class="hljs-title">voice_player</span>](#property-voice_player) | [AudioStreamPlayer](https://docs.godotengine.org/en/latest/classes/class_audiostreamplayer.html#class-audiostreamplayer) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span> | [<span class="hljs-title">get_remaining_time</span>](#method-get_remaining_time) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_running</span>](#method-is_running) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_voiced</span>](#method-is_voiced) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">pause</span>](#method-pause) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">play_voice</span>](#method-play_voice) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume</span>](#method-resume) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_bus</span>](#method-set_bus) ( `value`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_file</span>](#method-set_file) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_volume</span>](#method-set_volume) ( `value`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">stop_audio</span>](#method-stop_audio) ( ) 
--- 

## Signals


<a class="header" id="signal-voiceline_finished" href="#signal-voiceline_finished">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">voiceline_finished</span>](#signal-voiceline_finished) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-voiceline_started" href="#signal-voiceline_started">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">voiceline_started</span>](#signal-voiceline_started) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-voiceline_stopped" href="#signal-voiceline_stopped">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">voiceline_stopped</span>](#signal-voiceline_stopped) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-current_audio_file" href="#property-current_audio_file">**<span class="hljs-attribute">var</span> <span class="hljs-title">current_audio_file</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-voice_player" href="#property-voice_player">**<span class="hljs-attribute">var</span> <span class="hljs-title">voice_player</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-get_remaining_time" href="#method-get_remaining_time">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_remaining_time</span>](#method-get_remaining_time) ( )</a>  ⇒ <span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_running" href="#method-is_running">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_running</span>](#method-is_running) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_voiced" href="#method-is_voiced">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_voiced</span>](#method-is_voiced) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-pause" href="#method-pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pause</span>](#method-pause) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-play_voice" href="#method-play_voice">**<span class="hljs-attribute">func</span> [<span class="hljs-title">play_voice</span>](#method-play_voice) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-resume" href="#method-resume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume</span>](#method-resume) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_bus" href="#method-set_bus">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_bus</span>](#method-set_bus) ( `value`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_file" href="#method-set_file">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_file</span>](#method-set_file) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_volume" href="#method-set_volume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_volume</span>](#method-set_volume) ( `value`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-stop_audio" href="#method-stop_audio">**<span class="hljs-attribute">func</span> [<span class="hljs-title">stop_audio</span>](#method-stop_audio) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

