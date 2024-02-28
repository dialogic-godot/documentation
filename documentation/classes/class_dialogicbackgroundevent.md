
<div class="header-banner purple">
<div class="header-label purple">DialogicBackgroundEvent</div>
</div>

*This contains the source code documentation of the class `DialogicBackgroundEvent`.*
        
# DialogicBackgroundEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

# Settings
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">argument</span>](#property-argument) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">fade</span>](#property-fade) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
[<span class="hljs-title">scene</span>](#property-scene) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">transition</span>](#property-transition) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_shortcode</span>](#property-get_shortcode) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_transition_suggestions</span>](#property-get_transition_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
--- 
## Constants


<a class="header" id="constant-IMAGE" href="#constant-IMAGE">**<span class="hljs-attribute">const</span> <span class="hljs-title">IMAGE</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-CUSTOM" href="#constant-CUSTOM">**<span class="hljs-attribute">const</span> <span class="hljs-title">CUSTOM</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-DEFAULT" href="#constant-DEFAULT">**<span class="hljs-attribute">const</span> <span class="hljs-title">DEFAULT</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-CUSTOM" href="#constant-CUSTOM">**<span class="hljs-attribute">const</span> <span class="hljs-title">CUSTOM</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-argument" href="#property-argument">**<span class="hljs-attribute">var</span> <span class="hljs-title">argument</span> <span style = "color: gray"> = </span> ""** 



The argument that is passed to the background scene. For the default scene it's the path to the image to show.

---



<a class="header" id="property-fade" href="#property-fade">**<span class="hljs-attribute">var</span> <span class="hljs-title">fade</span> <span style = "color: gray"> = </span> 0.0** 



The time the fade animation will take. Leave at 0 for instant change.

---



<a class="header" id="property-scene" href="#property-scene">**<span class="hljs-attribute">var</span> <span class="hljs-title">scene</span> <span style = "color: gray"> = </span> ""** 



The scene to use. If empty, this will default to the DefaultBackground.gd scene. This scene supports images and fading. If you set it to a scene path, then that scene will be instanced. Learn more about custom backgrounds in the Subsystem_Background.gd docs.

---



<a class="header" id="property-transition" href="#property-transition">**<span class="hljs-attribute">var</span> <span class="hljs-title">transition</span> <span style = "color: gray"> = </span> ""** 



Name of the transition to use.

---

## Method Descriptions



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode" href="#method-get_shortcode">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode</span>](#property-get_shortcode) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode_parameters" href="#method-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_transition_suggestions" href="#method-get_transition_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_transition_suggestions</span>](#property-get_transition_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

