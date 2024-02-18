
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
action | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
animation_length | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.5` 
animation_name | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
animation_repeats | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `1` 
animation_wait | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
character | [DialogicCharacter](class_dialogiccharacter.md) |  `null` 
character_identifier | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
extra_data | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
mirrored | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
portrait | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
position | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `1` 
position_move_time | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.0` 
regex | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
set_mirrored | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
set_portrait | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
set_position | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
set_z_index | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
z_index | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
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



<a class="header" id="property-build_event_editor" href="#property-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-from_text" href="#property-from_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">from_text</span>](#property-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_animation_suggestions" href="#property-get_animation_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_animation_suggestions</span>](#property-get_animation_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_character_suggestions" href="#property-get_character_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_suggestions</span>](#property-get_character_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_portrait_suggestions" href="#property-get_portrait_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_portrait_suggestions</span>](#property-get_portrait_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_shortcode_parameters" href="#property-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



this is only here to provide a list of default values this way the module manager can add custom default overrides to this event. this is also why some properties are commented out, because it's not recommended to overwrite them this way

---



<a class="header" id="property-has_no_portraits" href="#property-has_no_portraits">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_no_portraits</span>](#property-has_no_portraits) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_valid_event" href="#property-is_valid_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_valid_event</span>](#property-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-should_show_animation_options" href="#property-should_show_animation_options">**<span class="hljs-attribute">func</span> [<span class="hljs-title">should_show_animation_options</span>](#property-should_show_animation_options) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-should_show_portrait_selector" href="#property-should_show_portrait_selector">**<span class="hljs-attribute">func</span> [<span class="hljs-title">should_show_portrait_selector</span>](#property-should_show_portrait_selector) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-to_text" href="#property-to_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">to_text</span>](#property-to_text) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

