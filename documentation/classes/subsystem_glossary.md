
<div class="header-banner purple">
<div class="header-label purple">Glossary</div>
</div>

*This contains the source code documentation of the class `subsystem_Glossary`.*
        
# subsystem_Glossary
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that handles glossaries.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">glossaries</span>](#property-glossaries) | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |  `[]` 
[<span class="hljs-title">enabled</span>](#property-enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">color_overrides</span>](#property-color_overrides) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{}` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">parse_glossary</span>](#method-parse_glossary) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_glossary</span>](#method-add_glossary) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[DialogicGlossary](class_dialogicglossary.md)</span> | [<span class="hljs-title">find_glossary</span>](#method-find_glossary) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_entry</span>](#method-get_entry) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">translate</span>](#method-translate) ( `tr_base`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `property`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname), `fallback_entry`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
--- 
## Constants


<a class="header" id="constant-SETTING_DEFAULT_COLOR" href="#constant-SETTING_DEFAULT_COLOR">**<span class="hljs-attribute">const</span> <span class="hljs-title">SETTING_DEFAULT_COLOR</span><span class="hljs-comment"> = "dialogic/glossary/default_color"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-glossaries" href="#property-glossaries">**<span class="hljs-attribute">var</span> <span class="hljs-title">glossaries</span> <span style = "color: gray"> = </span> []** 



List of glossary resources that are used.

---



<a class="header" id="property-enabled" href="#property-enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">enabled</span> <span style = "color: gray"> = </span> true** 



If false, no parsing will be done.

---



<a class="header" id="property-color_overrides" href="#property-color_overrides">**<span class="hljs-attribute">var</span> <span class="hljs-title">color_overrides</span> <span style = "color: gray"> = </span> {}** 



Any key in this dictionary will overwrite the color for any item with that name.

---

## Method Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-parse_glossary" href="#method-parse_glossary">**<span class="hljs-attribute">func</span> [<span class="hljs-title">parse_glossary</span>](#method-parse_glossary) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-add_glossary" href="#method-add_glossary">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_glossary</span>](#method-add_glossary) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-find_glossary" href="#method-find_glossary">**<span class="hljs-attribute">func</span> [<span class="hljs-title">find_glossary</span>](#method-find_glossary) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[DialogicGlossary](class_dialogicglossary.md)</span>** 



Iterates over all glossaries and returns the first one that matches the `entry_key`.  Runtime complexity: O(n), where n is the number of glossaries.

---



<a class="header" id="method-get_entry" href="#method-get_entry">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_entry</span>](#method-get_entry) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Returns the first match for a given entry key. If translation is available and enabled, it will be translated

---



<a class="header" id="method-translate" href="#method-translate">**<span class="hljs-attribute">func</span> [<span class="hljs-title">translate</span>](#method-translate) ( `tr_base`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `property`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname), `fallback_entry`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Tries to translate the property with the given

---

