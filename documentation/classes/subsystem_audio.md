
<div class="header-banner purple">
<div class="header-label purple">subsystem_Audio</div>
</div>

*This contains the source code documentation of the class `subsystem_Audio`.*
        
# subsystem_Audio
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem for managing background music and one-shot sound effects.
## Description
This subsystem has many different helper methods for managing audio in your timeline. For instance, you can listen to music changes via [music_started](#signal-music_started).

## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">base_music_player</span>](#property-base_music_player) | [AudioStreamPlayer](https://docs.godotengine.org/en/latest/classes/class_audiostreamplayer.html#class-audiostreamplayer) |   
[<span class="hljs-title">base_sound_player</span>](#property-base_sound_player) | [AudioStreamPlayer](https://docs.godotengine.org/en/latest/classes/class_audiostreamplayer.html#class-audiostreamplayer) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_music</span>](#method-has_music) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">interpolate_volume_linearly</span>](#method-interpolate_volume_linearly) ( `value`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float), `node`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_music_playing_resource</span>](#method-is_music_playing_resource) ( `resource_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">pause</span>](#method-pause) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">play_sound</span>](#method-play_sound) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `volume`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `audio_bus`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `"Master"`, `loop`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume</span>](#method-resume) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">stop_all_sounds</span>](#method-stop_all_sounds) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_music</span>](#method-update_music) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `volume`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `audio_bus`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `"Master"`, `fade_time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `loop`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
--- 

## Signals


<a class="header" id="signal-music_started" href="#signal-music_started">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">music_started</span>](#signal-music_started) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 Whenever a new background is set, this signal is emitted and contains a dictionary with the following keys: 

Key         |   Value Type  | Value 
----------- | ------------- | ----- 
`path`      | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) | The path to the audio resource file. 
`volume`    | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)  | The volume of the audio resource that will be set to the audio player. 
`audio_bus` | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) | The audio bus name that the audio player will use. 
`loop`      | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)   | Whether the audio resource will loop or not once it finishes playing. 
 

---



<a class="header" id="signal-sound_started" href="#signal-sound_started">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">sound_started</span>](#signal-sound_started) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 Whenever a new sound effect is set, this signal is emitted and contains a dictionary with the following keys: 

Key         |   Value Type  | Value 
----------- | ------------- | ----- 
`path`      | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) | The path to the audio resource file. 
`volume`    | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)  | The volume of the audio resource that will be set to the audio player. 
`audio_bus` | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) | The audio bus name that the audio player will use. 
`loop`      | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)   | Whether the audio resource will loop or not once it finishes playing. 
] 

---

## Property Descriptions



<a class="header" id="property-base_music_player" href="#property-base_music_player">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_music_player</span> <span style = "color: gray"> = </span> <unknown>** 



Audio player used to play background music. Background music is long audio.

---



<a class="header" id="property-base_sound_player" href="#property-base_sound_player">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_sound_player</span> <span style = "color: gray"> = </span> <unknown>** 



Audio player used to play sound effects. Sound effects are short audio.

---

## Method Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Clears the state on this subsystem and stops the all sounds.  If you want to stop audio only, use [stop_all_sounds](#property-stop_all_sounds).

---



<a class="header" id="method-has_music" href="#method-has_music">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_music</span>](#method-has_music) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Whether music is playing.

---



<a class="header" id="method-interpolate_volume_linearly" href="#method-interpolate_volume_linearly">**<span class="hljs-attribute">func</span> [<span class="hljs-title">interpolate_volume_linearly</span>](#method-interpolate_volume_linearly) ( `value`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float), `node`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) )</a>  ⇒ <span style = "color: gray">void</span>** 



Converts a linear loudness value to decibel and sets that volume to the given `node`.

---



<a class="header" id="method-is_music_playing_resource" href="#method-is_music_playing_resource">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_music_playing_resource</span>](#method-is_music_playing_resource) ( `resource_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns whether the currently playing audio resource is the same as this event's `resource_path`.

---



<a class="header" id="method-load_game_state" href="#method-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Loads the state on this subsystem from the current state info.

---



<a class="header" id="method-pause" href="#method-pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pause</span>](#method-pause) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Pauses playing audio.

---



<a class="header" id="method-play_sound" href="#method-play_sound">**<span class="hljs-attribute">func</span> [<span class="hljs-title">play_sound</span>](#method-play_sound) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `volume`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `audio_bus`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `"Master"`, `loop`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



Plays a given sound file.

---



<a class="header" id="method-resume" href="#method-resume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume</span>](#method-resume) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Resumes playing audio.

---



<a class="header" id="method-stop_all_sounds" href="#method-stop_all_sounds">**<span class="hljs-attribute">func</span> [<span class="hljs-title">stop_all_sounds</span>](#method-stop_all_sounds) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Stops all audio.

---



<a class="header" id="method-update_music" href="#method-update_music">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_music</span>](#method-update_music) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `volume`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `audio_bus`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `"Master"`, `fade_time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `loop`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span style = "color: gray">void</span>** 



Updates the background music. Will fade out previous music.

---

