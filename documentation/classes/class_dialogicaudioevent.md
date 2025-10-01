
<div class="header-banner purple">
<div class="header-label purple">DialogicAudioEvent</div>
</div>

*This contains the source code documentation of the class `DialogicAudioEvent`.*
        
# DialogicAudioEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

Event that can play audio on a channel. The channel can be prededinfed (with default settings defined in the settings) or created on the spot. If no channel is given will play as a One-Shot SFX.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">file_path</span>](#property-file_path) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">channel_name</span>](#property-channel_name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">fade_length</span>](#property-fade_length) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
[<span class="hljs-title">volume</span>](#property-volume) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
[<span class="hljs-title">audio_bus</span>](#property-audio_bus) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">loop</span>](#property-loop) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">sync_channel</span>](#property-sync_channel) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">set_fade_length</span>](#property-set_fade_length) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">set_volume</span>](#property-set_volume) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">set_audio_bus</span>](#property-set_audio_bus) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">set_loop</span>](#property-set_loop) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">set_sync_channel</span>](#property-set_sync_channel) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">regex</span>](#property-regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |  `create_from_string(...)` 
[<span class="hljs-title">channel_name_regex</span>](#property-channel_name_regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |  `create_from_string(...)` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">to_text</span>](#method-to_text) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">store_to_shortcode_parameters</span>](#method-store_to_shortcode_parameters) ( `params`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_channel_defaults</span>](#method-has_channel_defaults) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_audio_channel_suggestions</span>](#method-get_audio_channel_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_sync_audio_channel_suggestions</span>](#method-get_sync_audio_channel_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
--- 
## Property Descriptions



<a class="header" id="property-file_path" href="#property-file_path">**<span class="hljs-attribute">var</span> <span class="hljs-title">file_path</span> <span style = "color: gray"> = </span> ""** 



The file to play. If empty, the previous audio will be faded out.

---



<a class="header" id="property-channel_name" href="#property-channel_name">**<span class="hljs-attribute">var</span> <span class="hljs-title">channel_name</span> <span style = "color: gray"> = </span> ""** 



The channel name to use. If none given plays as a One-Shot SFX.

---



<a class="header" id="property-fade_length" href="#property-fade_length">**<span class="hljs-attribute">var</span> <span class="hljs-title">fade_length</span> <span style = "color: gray"> = </span> 0.0** 



The length of the fade. If 0 it's an instant change.

---



<a class="header" id="property-volume" href="#property-volume">**<span class="hljs-attribute">var</span> <span class="hljs-title">volume</span> <span style = "color: gray"> = </span> 0.0** 



The volume in decibel.

---



<a class="header" id="property-audio_bus" href="#property-audio_bus">**<span class="hljs-attribute">var</span> <span class="hljs-title">audio_bus</span> <span style = "color: gray"> = </span> ""** 



The audio bus the audio will be played on.

---



<a class="header" id="property-loop" href="#property-loop">**<span class="hljs-attribute">var</span> <span class="hljs-title">loop</span> <span style = "color: gray"> = </span> true** 



If true, the audio will loop, otherwise only play once.

---



<a class="header" id="property-sync_channel" href="#property-sync_channel">**<span class="hljs-attribute">var</span> <span class="hljs-title">sync_channel</span> <span style = "color: gray"> = </span> ""** 



Sync starting time with different channel (if playing audio on that channel)

---



<a class="header" id="property-set_fade_length" href="#property-set_fade_length">**<span class="hljs-attribute">var</span> <span class="hljs-title">set_fade_length</span> <span style = "color: gray"> = </span> false** 



Helpers. Set automatically

---



<a class="header" id="property-set_volume" href="#property-set_volume">**<span class="hljs-attribute">var</span> <span class="hljs-title">set_volume</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_audio_bus" href="#property-set_audio_bus">**<span class="hljs-attribute">var</span> <span class="hljs-title">set_audio_bus</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_loop" href="#property-set_loop">**<span class="hljs-attribute">var</span> <span class="hljs-title">set_loop</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_sync_channel" href="#property-set_sync_channel">**<span class="hljs-attribute">var</span> <span class="hljs-title">set_sync_channel</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-regex" href="#property-regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">regex</span> <span style = "color: gray"> = </span> create_from_string(...)** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-channel_name_regex" href="#property-channel_name_regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">channel_name_regex</span> <span style = "color: gray"> = </span> create_from_string(...)** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-to_text" href="#method-to_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">to_text</span>](#method-to_text) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-from_text" href="#method-from_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode_parameters" href="#method-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-store_to_shortcode_parameters" href="#method-store_to_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">store_to_shortcode_parameters</span>](#method-store_to_shortcode_parameters) ( `params`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}` )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns a string with all the shortcode parameters.

---



<a class="header" id="method-is_valid_event" href="#method-is_valid_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-has_channel_defaults" href="#method-has_channel_defaults">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_channel_defaults</span>](#method-has_channel_defaults) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Helper for the visibility conditions

---



<a class="header" id="method-get_audio_channel_suggestions" href="#method-get_audio_channel_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_audio_channel_suggestions</span>](#method-get_audio_channel_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_sync_audio_channel_suggestions" href="#method-get_sync_audio_channel_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_sync_audio_channel_suggestions</span>](#method-get_sync_audio_channel_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

