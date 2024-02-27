
<div class="header-banner purple">
<div class="header-label purple">DialogicCharacterEvent</div>
</div>

*This contains the source code documentation of the class `DialogicCharacterEvent`.*
        
# DialogicCharacterEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

# Settings
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">action</span>](#property-action) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">animation_length</span>](#property-animation_length) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.5` 
[<span class="hljs-title">animation_name</span>](#property-animation_name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">animation_repeats</span>](#property-animation_repeats) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `1` 
[<span class="hljs-title">animation_wait</span>](#property-animation_wait) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">character</span>](#property-character) | [DialogicCharacter](class_dialogiccharacter.md) |  `null` 
[<span class="hljs-title">character_identifier</span>](#property-character_identifier) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
[<span class="hljs-title">extra_data</span>](#property-extra_data) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">mirrored</span>](#property-mirrored) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">portrait</span>](#property-portrait) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">position</span>](#property-position) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `1` 
[<span class="hljs-title">position_move_time</span>](#property-position_move_time) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
[<span class="hljs-title">regex</span>](#property-regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
[<span class="hljs-title">set_mirrored</span>](#property-set_mirrored) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">set_portrait</span>](#property-set_portrait) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">set_position</span>](#property-set_position) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">set_z_index</span>](#property-set_z_index) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">z_index</span>](#property-z_index) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#property-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_animation_suggestions</span>](#property-get_animation_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_character_suggestions</span>](#property-get_character_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_portrait_suggestions</span>](#property-get_portrait_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_no_portraits</span>](#property-has_no_portraits) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_valid_event</span>](#property-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">should_show_animation_options</span>](#property-should_show_animation_options) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">should_show_portrait_selector</span>](#property-should_show_portrait_selector) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">to_text</span>](#property-to_text) ( ) 
--- 
## Constants


<a class="header" id="constant-JOIN" href="#constant-JOIN">**<span class="hljs-attribute">const</span> <span class="hljs-title">JOIN</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-LEAVE" href="#constant-LEAVE">**<span class="hljs-attribute">const</span> <span class="hljs-title">LEAVE</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-UPDATE" href="#constant-UPDATE">**<span class="hljs-attribute">const</span> <span class="hljs-title">UPDATE</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-action" href="#property-action">**<span class="hljs-attribute">var</span> <span class="hljs-title">action</span> <span style = "color: gray"> = </span> 0** 



The type of action of this event (JOIN/LEAVE/UPDATE). See [Actions].

---



<a class="header" id="property-animation_length" href="#property-animation_length">**<span class="hljs-attribute">var</span> <span class="hljs-title">animation_length</span> <span style = "color: gray"> = </span> 0.5** 



Length of the animation.

---



<a class="header" id="property-animation_name" href="#property-animation_name">**<span class="hljs-attribute">var</span> <span class="hljs-title">animation_name</span> <span style = "color: gray"> = </span> ""** 



Name of the animation script (extending DialogicAnimation). On Join/Leave empty (default) will fallback to the animations set in the settings. On Update empty will mean no animation.

---



<a class="header" id="property-animation_repeats" href="#property-animation_repeats">**<span class="hljs-attribute">var</span> <span class="hljs-title">animation_repeats</span> <span style = "color: gray"> = </span> 1** 



How often the animation is repeated. Only for Update events.

---



<a class="header" id="property-animation_wait" href="#property-animation_wait">**<span class="hljs-attribute">var</span> <span class="hljs-title">animation_wait</span> <span style = "color: gray"> = </span> false** 



If true, the events waits for the animation to finish before the next event starts.

---



<a class="header" id="property-character" href="#property-character">**<span class="hljs-attribute">var</span> <span class="hljs-title">character</span> <span style = "color: gray"> = </span> null** 



The character that will join/leave/update.

---



<a class="header" id="property-character_identifier" href="#property-character_identifier">**<span class="hljs-attribute">var</span> <span class="hljs-title">character_identifier</span>** 



Used to set the character resource from the unique name identifier and vice versa

---



<a class="header" id="property-extra_data" href="#property-extra_data">**<span class="hljs-attribute">var</span> <span class="hljs-title">extra_data</span> <span style = "color: gray"> = </span> ""** 



If set, will be passed to the portrait scene.

---



<a class="header" id="property-mirrored" href="#property-mirrored">**<span class="hljs-attribute">var</span> <span class="hljs-title">mirrored</span> <span style = "color: gray"> = </span> false** 



If true, the portrait will be set to mirrored.

---



<a class="header" id="property-portrait" href="#property-portrait">**<span class="hljs-attribute">var</span> <span class="hljs-title">portrait</span> <span style = "color: gray"> = </span> ""** 



For Join/Update, this will be the portrait of the character that is shown. Not used on Leave. If empty, the default portrait will be used.

---



<a class="header" id="property-position" href="#property-position">**<span class="hljs-attribute">var</span> <span class="hljs-title">position</span> <span style = "color: gray"> = </span> 1** 



The index of the position this character should move to

---



<a class="header" id="property-position_move_time" href="#property-position_move_time">**<span class="hljs-attribute">var</span> <span class="hljs-title">position_move_time</span> <span style = "color: gray"> = </span> 0.0** 



For Update only. If bigger then 0, the portrait will tween to the new position (if changed) in this time (in seconds).

---



<a class="header" id="property-regex" href="#property-regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">regex</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_mirrored" href="#property-set_mirrored">**<span class="hljs-attribute">var</span> <span class="hljs-title">set_mirrored</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_portrait" href="#property-set_portrait">**<span class="hljs-attribute">var</span> <span class="hljs-title">set_portrait</span> <span style = "color: gray"> = </span> false** 



Indicators for whether something should be updated (UPDATE mode only)

---



<a class="header" id="property-set_position" href="#property-set_position">**<span class="hljs-attribute">var</span> <span class="hljs-title">set_position</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_z_index" href="#property-set_z_index">**<span class="hljs-attribute">var</span> <span class="hljs-title">set_z_index</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-z_index" href="#property-z_index">**<span class="hljs-attribute">var</span> <span class="hljs-title">z_index</span> <span style = "color: gray"> = </span> 0** 



The z_index that the portrait should have.

---

## Methods Descriptions



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-from_text" href="#method-from_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">from_text</span>](#property-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_animation_suggestions" href="#method-get_animation_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_animation_suggestions</span>](#property-get_animation_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_character_suggestions" href="#method-get_character_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_suggestions</span>](#property-get_character_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_portrait_suggestions" href="#method-get_portrait_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_portrait_suggestions</span>](#property-get_portrait_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode_parameters" href="#method-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



this is only here to provide a list of default values this way the module manager can add custom default overrides to this event. this is also why some properties are commented out, because it's not recommended to overwrite them this way

---



<a class="header" id="method-has_no_portraits" href="#method-has_no_portraits">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_no_portraits</span>](#property-has_no_portraits) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_valid_event" href="#method-is_valid_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_valid_event</span>](#property-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-should_show_animation_options" href="#method-should_show_animation_options">**<span class="hljs-attribute">func</span> [<span class="hljs-title">should_show_animation_options</span>](#property-should_show_animation_options) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-should_show_portrait_selector" href="#method-should_show_portrait_selector">**<span class="hljs-attribute">func</span> [<span class="hljs-title">should_show_portrait_selector</span>](#property-should_show_portrait_selector) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-to_text" href="#method-to_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">to_text</span>](#property-to_text) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

