
<div class="header-banner purple">
<div class="header-label purple">DialogicMusicEvent</div>
</div>

*This contains the source code documentation of the class `DialogicMusicEvent`.*
        
# DialogicMusicEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

# Settings
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">audio_bus</span>](#property-audio_bus) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"Master"` 
[<span class="hljs-title">fade_length</span>](#property-fade_length) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
[<span class="hljs-title">file_path</span>](#property-file_path) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">loop</span>](#property-loop) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">volume</span>](#property-volume) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_bus_suggestions</span>](#property-get_bus_suggestions) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_shortcode</span>](#property-get_shortcode) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( ) 
--- 
## Property Descriptions



<a class="header" id="property-audio_bus" href="#property-audio_bus">**<span class="hljs-attribute">var</span> <span class="hljs-title">audio_bus</span> <span style = "color: gray"> = </span> "Master"** 



The audio bus the music will be played at.

---



<a class="header" id="property-fade_length" href="#property-fade_length">**<span class="hljs-attribute">var</span> <span class="hljs-title">fade_length</span> <span style = "color: gray"> = </span> 0.0** 



The length of the fade. If 0 (by default) it's an instant change.

---



<a class="header" id="property-file_path" href="#property-file_path">**<span class="hljs-attribute">var</span> <span class="hljs-title">file_path</span> <span style = "color: gray"> = </span> ""** 



The file to play. If empty, the previous music will be faded out.

---



<a class="header" id="property-loop" href="#property-loop">**<span class="hljs-attribute">var</span> <span class="hljs-title">loop</span> <span style = "color: gray"> = </span> true** 



If true, the audio will loop, otherwise only play once.

---



<a class="header" id="property-volume" href="#property-volume">**<span class="hljs-attribute">var</span> <span class="hljs-title">volume</span> <span style = "color: gray"> = </span> 0.0** 



The volume the music will be played at.

---

## Method Descriptions



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_bus_suggestions" href="#method-get_bus_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_bus_suggestions</span>](#property-get_bus_suggestions) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode" href="#method-get_shortcode">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode</span>](#property-get_shortcode) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode_parameters" href="#method-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

