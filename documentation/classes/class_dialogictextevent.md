
<div class="header-banner purple">
<div class="header-label purple">DialogicTextEvent</div>
</div>

*This contains the source code documentation of the class `DialogicTextEvent`.*
        
# DialogicTextEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

# Settings
## Properties
Name | Type | Default 
--- | --- | --- 
character | [DialogicCharacter](class_dialogiccharacter.md) |  `null` 
character_identifier | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
completion_text_character_getter_regex | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
completion_text_effects | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
portrait | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
regex | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
split_regex | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
state | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `1` 
text | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
text_effect_color | [Color](https://docs.godotengine.org/en/latest/classes/class_color.html#class-color) |  `Color(0.537255, 0.509804, 0.462745, 1)` 
text_effects | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
text_effects_regex | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
text_random_word_regex | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">do_any_characters_exist</span>](#property-do_any_characters_exist) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">end_text_event</span>](#property-end_text_event) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">from_text</span>](#property-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_character_suggestions</span>](#property-get_character_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_portrait_suggestions</span>](#property-get_portrait_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">has_no_portraits</span>](#property-has_no_portraits) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">is_string_full_event</span>](#property-is_string_full_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">is_valid_event</span>](#property-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">load_text_effects</span>](#property-load_text_effects) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">suggest_bbcode</span>](#property-suggest_bbcode) ( `text`: [CodeEdit](https://docs.godotengine.org/en/latest/classes/class_codeedit.html#class-codeedit) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">to_text</span>](#property-to_text) ( ) 
--- 
## Constants


<a class="header" id="constant-REVEALING" href="#constant-REVEALING">**<span class="hljs-attribute">const</span> <span class="hljs-title">REVEALING</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-IDLE" href="#constant-IDLE">**<span class="hljs-attribute">const</span> <span class="hljs-title">IDLE</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-DONE" href="#constant-DONE">**<span class="hljs-attribute">const</span> <span class="hljs-title">DONE</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-advance" href="#signal-advance">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">advance</span>](#signal-advance) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-build_event_editor" href="#property-build_event_editor">**<span class="hljs-attribute">void</span> [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-do_any_characters_exist" href="#property-do_any_characters_exist">**<span class="hljs-attribute">void</span> [<span class="hljs-title">do_any_characters_exist</span>](#property-do_any_characters_exist) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-end_text_event" href="#property-end_text_event">**<span class="hljs-attribute">void</span> [<span class="hljs-title">end_text_event</span>](#property-end_text_event) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-from_text" href="#property-from_text">**<span class="hljs-attribute">void</span> [<span class="hljs-title">from_text</span>](#property-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_character_suggestions" href="#property-get_character_suggestions">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_character_suggestions</span>](#property-get_character_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_portrait_suggestions" href="#property-get_portrait_suggestions">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_portrait_suggestions</span>](#property-get_portrait_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_shortcode_parameters" href="#property-get_shortcode_parameters">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-has_no_portraits" href="#property-has_no_portraits">**<span class="hljs-attribute">void</span> [<span class="hljs-title">has_no_portraits</span>](#property-has_no_portraits) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_string_full_event" href="#property-is_string_full_event">**<span class="hljs-attribute">void</span> [<span class="hljs-title">is_string_full_event</span>](#property-is_string_full_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_valid_event" href="#property-is_valid_event">**<span class="hljs-attribute">void</span> [<span class="hljs-title">is_valid_event</span>](#property-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-load_text_effects" href="#property-load_text_effects">**<span class="hljs-attribute">void</span> [<span class="hljs-title">load_text_effects</span>](#property-load_text_effects) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-suggest_bbcode" href="#property-suggest_bbcode">**<span class="hljs-attribute">void</span> [<span class="hljs-title">suggest_bbcode</span>](#property-suggest_bbcode) ( `text`: [CodeEdit](https://docs.godotengine.org/en/latest/classes/class_codeedit.html#class-codeedit) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-to_text" href="#property-to_text">**<span class="hljs-attribute">void</span> [<span class="hljs-title">to_text</span>](#property-to_text) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

