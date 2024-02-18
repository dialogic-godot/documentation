
<div class="header-banner purple">
<div class="header-label purple">subsystem_voice</div>
</div>

*This contains the source code documentation of the class `subsystem_voice`.*
        
# subsystem_voice
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

##################################################################################################
## Properties
Name | Type | Default 
--- | --- | --- 
current_audio_file | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
voice_player | [AudioStreamPlayer](https://docs.godotengine.org/en/latest/classes/class_audiostreamplayer.html#class-audiostreamplayer) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span> | [<span class="hljs-title">get_remaining_time</span>](#property-get_remaining_time) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_running</span>](#property-is_running) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_voiced</span>](#property-is_voiced) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">pause</span>](#property-pause) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">play_voice</span>](#property-play_voice) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume</span>](#property-resume) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_bus</span>](#property-set_bus) ( `value`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_file</span>](#property-set_file) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_volume</span>](#property-set_volume) ( `value`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">stop_audio</span>](#property-stop_audio) ( ) 
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



<a class="header" id="property-get_remaining_time" href="#property-get_remaining_time">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_remaining_time</span>](#property-get_remaining_time) ( )</a>  ⇒ <span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_running" href="#property-is_running">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_running</span>](#property-is_running) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_voiced" href="#property-is_voiced">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_voiced</span>](#property-is_voiced) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-pause" href="#property-pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pause</span>](#property-pause) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-play_voice" href="#property-play_voice">**<span class="hljs-attribute">func</span> [<span class="hljs-title">play_voice</span>](#property-play_voice) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-resume" href="#property-resume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume</span>](#property-resume) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_bus" href="#property-set_bus">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_bus</span>](#property-set_bus) ( `value`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_file" href="#property-set_file">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_file</span>](#property-set_file) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_volume" href="#property-set_volume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_volume</span>](#property-set_volume) ( `value`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-stop_audio" href="#property-stop_audio">**<span class="hljs-attribute">func</span> [<span class="hljs-title">stop_audio</span>](#property-stop_audio) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

