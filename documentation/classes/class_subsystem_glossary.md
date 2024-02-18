
<div class="header-banner purple">
<div class="header-label purple">subsystem_glossary</div>
</div>

*This contains the source code documentation of the class `subsystem_glossary`.*
        
# subsystem_glossary
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that handles glossaries.
## Properties
Name | Type | Default 
--- | --- | --- 
color_overrides | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
enabled | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
glossaries | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_glossary</span>](#property-add_glossary) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[DialogicGlossary](class_dialogicglossary.md)</span> | [<span class="hljs-title">find_glossary</span>](#property-find_glossary) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">parse_glossary</span>](#property-parse_glossary) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
--- 
## Property Descriptions



<a class="header" id="property-add_glossary" href="#property-add_glossary">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_glossary</span>](#property-add_glossary) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-clear_game_state" href="#property-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-find_glossary" href="#property-find_glossary">**<span class="hljs-attribute">func</span> [<span class="hljs-title">find_glossary</span>](#property-find_glossary) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[DialogicGlossary](class_dialogicglossary.md)</span>** 



Iterates over all glossaries and returns the first one that matches the `entry_key`.  Returns null if none of the glossaries has an entry with that key. If translation is enabled, uses the `entry_key` as well to check `_translation_keys`.  Runtime complexity: O(n), where n is the number of glossaries.

---



<a class="header" id="property-parse_glossary" href="#property-parse_glossary">**<span class="hljs-attribute">func</span> [<span class="hljs-title">parse_glossary</span>](#property-parse_glossary) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

