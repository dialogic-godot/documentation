
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
[<span class="hljs-title">character</span>](#property-character) | [DialogicCharacter](class_dialogiccharacter.md) |  `null` 
[<span class="hljs-title">character_identifier</span>](#property-character_identifier) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
[<span class="hljs-title">completion_text_character_getter_regex</span>](#property-completion_text_character_getter_regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
[<span class="hljs-title">completion_text_effects</span>](#property-completion_text_effects) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">portrait</span>](#property-portrait) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">regex</span>](#property-regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
[<span class="hljs-title">split_regex</span>](#property-split_regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
[<span class="hljs-title">state</span>](#property-state) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `1` 
[<span class="hljs-title">text</span>](#property-text) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">text_effect_color</span>](#property-text_effect_color) | [Color](https://docs.godotengine.org/en/latest/classes/class_color.html#class-color) |  `Color(0.537255, 0.509804, 0.462745, 1)` 
[<span class="hljs-title">text_effects</span>](#property-text_effects) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">text_effects_regex</span>](#property-text_effects_regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
[<span class="hljs-title">text_random_word_regex</span>](#property-text_random_word_regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">do_any_characters_exist</span>](#method-do_any_characters_exist) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">end_text_event</span>](#method-end_text_event) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_character_suggestions</span>](#method-get_character_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_portrait_suggestions</span>](#method-get_portrait_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_no_portraits</span>](#method-has_no_portraits) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_string_full_event</span>](#method-is_string_full_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_text_effects</span>](#method-load_text_effects) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">suggest_bbcode</span>](#method-suggest_bbcode) ( `text`: [CodeEdit](https://docs.godotengine.org/en/latest/classes/class_codeedit.html#class-codeedit) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">to_text</span>](#method-to_text) ( ) 
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



<a class="header" id="property-character" href="#property-character">**<span class="hljs-attribute">var</span> <span class="hljs-title">character</span> <span style = "color: gray"> = </span> null** 



If this is not null, the given character (as a resource) will be associated with this event. The DialogicNode_NameLabel will show the characters display_name. If a typing sound is setup, it will play.

---



<a class="header" id="property-character_identifier" href="#property-character_identifier">**<span class="hljs-attribute">var</span> <span class="hljs-title">character_identifier</span>** 



Used to set the character resource from the unique name identifier and vice versa

---



<a class="header" id="property-completion_text_character_getter_regex" href="#property-completion_text_character_getter_regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">completion_text_character_getter_regex</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-completion_text_effects" href="#property-completion_text_effects">**<span class="hljs-attribute">var</span> <span class="hljs-title">completion_text_effects</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-portrait" href="#property-portrait">**<span class="hljs-attribute">var</span> <span class="hljs-title">portrait</span> <span style = "color: gray"> = </span> ""** 



If a character is set, this setting can change the portrait of that character.

---



<a class="header" id="property-regex" href="#property-regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">regex</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-split_regex" href="#property-split_regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">split_regex</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-state" href="#property-state">**<span class="hljs-attribute">var</span> <span class="hljs-title">state</span> <span style = "color: gray"> = </span> 1** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text" href="#property-text">**<span class="hljs-attribute">var</span> <span class="hljs-title">text</span> <span style = "color: gray"> = </span> ""** 



This is the content of the text event. It is supposed to be displayed by a DialogicNode_DialogText node. That means you can use bbcode, but also some custom commands.

---



<a class="header" id="property-text_effect_color" href="#property-text_effect_color">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_effect_color</span> <span style = "color: gray"> = </span> Color(0.537255, 0.509804, 0.462745, 1)** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text_effects" href="#property-text_effects">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_effects</span> <span style = "color: gray"> = </span> ""** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text_effects_regex" href="#property-text_effects_regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_effects_regex</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text_random_word_regex" href="#property-text_random_word_regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_random_word_regex</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-do_any_characters_exist" href="#method-do_any_characters_exist">**<span class="hljs-attribute">func</span> [<span class="hljs-title">do_any_characters_exist</span>](#method-do_any_characters_exist) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-end_text_event" href="#method-end_text_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">end_text_event</span>](#method-end_text_event) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-from_text" href="#method-from_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_character_suggestions" href="#method-get_character_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_suggestions</span>](#method-get_character_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_portrait_suggestions" href="#method-get_portrait_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_portrait_suggestions</span>](#method-get_portrait_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode_parameters" href="#method-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-has_no_portraits" href="#method-has_no_portraits">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_no_portraits</span>](#method-has_no_portraits) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_string_full_event" href="#method-is_string_full_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_string_full_event</span>](#method-is_string_full_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_valid_event" href="#method-is_valid_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-load_text_effects" href="#method-load_text_effects">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_text_effects</span>](#method-load_text_effects) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-suggest_bbcode" href="#method-suggest_bbcode">**<span class="hljs-attribute">func</span> [<span class="hljs-title">suggest_bbcode</span>](#method-suggest_bbcode) ( `text`: [CodeEdit](https://docs.godotengine.org/en/latest/classes/class_codeedit.html#class-codeedit) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-to_text" href="#method-to_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">to_text</span>](#method-to_text) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

