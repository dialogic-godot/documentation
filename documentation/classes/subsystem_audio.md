
<div class="header-banner purple">
<div class="header-label purple">Audio</div>
</div>

*This contains the source code documentation of the class `subsystem_Audio`.*
        
# subsystem_Audio
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem for managing background audio and one-shot sound effects.
## Description
This subsystem has many different helper methods for managing audio in your timeline. For instance, you can listen to audio changes via [audio_started](#signal-audio_started).

## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">audio_node</span>](#property-audio_node) | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |  `new()` 
[<span class="hljs-title">one_shot_audio_node</span>](#property-one_shot_audio_node) | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |  `new()` 
[<span class="hljs-title">current_audio_channels</span>](#property-current_audio_channels) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{}` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">pause</span>](#method-pause) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume</span>](#method-resume) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_audio</span>](#method-update_audio) ( `channel_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `settings_overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_channel_playing</span>](#method-is_channel_playing) ( `channel_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">stop_all_channels</span>](#method-stop_all_channels) ( `fade`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">stop_all_one_shot_sounds</span>](#method-stop_all_one_shot_sounds) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">interpolate_volume_linearly</span>](#method-interpolate_volume_linearly) ( `value`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float), `node`: [AudioStreamPlayer](https://docs.godotengine.org/en/latest/classes/class_audiostreamplayer.html#class-audiostreamplayer) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_channel_playing_file</span>](#method-is_channel_playing_file) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `channel_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_any_channel_playing</span>](#method-is_any_channel_playing) ( ) 
--- 

## Signals


<a class="header" id="signal-audio_started" href="#signal-audio_started">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">audio_started</span>](#signal-audio_started) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 Whenever a new audio event is started, this signal is emitted and contains a dictionary with the following keys: 

Key         |   Value Type  | Value 
----------- | ------------- | ----- 
`path`      | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) | The path to the audio resource file. 
`channel`   | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) | The channel name to play the audio on. 
`volume`    | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)  | The volume in `db` of the audio resource that will be set to the . 
`audio_bus` | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) | The audio bus name that the  will use. 
`loop`      | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)   | Whether the audio resource will loop or not once it finishes playing. 
 

---

## Property Descriptions



<a class="header" id="property-audio_node" href="#property-audio_node">**<span class="hljs-attribute">var</span> <span class="hljs-title">audio_node</span> <span style = "color: gray"> = </span> new()** 



Audio node for holding audio players

---



<a class="header" id="property-one_shot_audio_node" href="#property-one_shot_audio_node">**<span class="hljs-attribute">var</span> <span class="hljs-title">one_shot_audio_node</span> <span style = "color: gray"> = </span> new()** 



Sound node for holding sound players

---



<a class="header" id="property-current_audio_channels" href="#property-current_audio_channels">**<span class="hljs-attribute">var</span> <span class="hljs-title">current_audio_channels</span> <span style = "color: gray"> = </span> {}** 



Dictionary with info of all current audio channels

---

## Method Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Clears the state on this subsystem and stops all audio.

---



<a class="header" id="method-load_game_state" href="#method-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Loads the state on this subsystem from the current state info.

---



<a class="header" id="method-pause" href="#method-pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pause</span>](#method-pause) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Pauses playing audio.

---



<a class="header" id="method-resume" href="#method-resume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume</span>](#method-resume) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Resumes playing audio.

---



<a class="header" id="method-update_audio" href="#method-update_audio">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_audio</span>](#method-update_audio) ( `channel_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `settings_overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}` )</a>  ⇒ <span style = "color: gray">void</span>** 



Plays the given file (or nothing) on the given channel. No channel given defaults to the "One-Shot SFX" channel, which does not save audio but can have multiple audios playing simultaneously.

---



<a class="header" id="method-is_channel_playing" href="#method-is_channel_playing">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_channel_playing</span>](#method-is_channel_playing) ( `channel_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns `true` if any audio is playing on the given `channel_name`.

---



<a class="header" id="method-stop_all_channels" href="#method-stop_all_channels">**<span class="hljs-attribute">func</span> [<span class="hljs-title">stop_all_channels</span>](#method-stop_all_channels) ( `fade`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Stops audio on all channels.

---



<a class="header" id="method-stop_all_one_shot_sounds" href="#method-stop_all_one_shot_sounds">**<span class="hljs-attribute">func</span> [<span class="hljs-title">stop_all_one_shot_sounds</span>](#method-stop_all_one_shot_sounds) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



# Stops all one-shot sounds.

---



<a class="header" id="method-interpolate_volume_linearly" href="#method-interpolate_volume_linearly">**<span class="hljs-attribute">func</span> [<span class="hljs-title">interpolate_volume_linearly</span>](#method-interpolate_volume_linearly) ( `value`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float), `node`: [AudioStreamPlayer](https://docs.godotengine.org/en/latest/classes/class_audiostreamplayer.html#class-audiostreamplayer) )</a>  ⇒ <span style = "color: gray">void</span>** 



Converts a linear loudness value to decibel and sets that volume to the given `node`.

---



<a class="header" id="method-is_channel_playing_file" href="#method-is_channel_playing_file">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_channel_playing_file</span>](#method-is_channel_playing_file) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `channel_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns whether the currently playing audio resource is the same as this event's `resource_path`, for `channel_name`.

---



<a class="header" id="method-is_any_channel_playing" href="#method-is_any_channel_playing">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_any_channel_playing</span>](#method-is_any_channel_playing) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns `true` if any channel is playing.

---

