
<div class="header-banner purple">
<div class="header-label purple">DialogicGlossary</div>
</div>

*This contains the source code documentation of the class `DialogicGlossary`.*
        
# DialogicGlossary
**Inherits:** [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource)

Resource used to store glossary entries. Can be saved to disc and used as a glossary. Add/create glossaries fom the glossaries editor
## Properties
Name | Type | Default 
--- | --- | --- 
enabled | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
entries | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_translation_id</span>](#property-add_translation_id) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">clear_translation_keys</span>](#property-clear_translation_keys) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_entry</span>](#property-get_entry) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_property_translation_key</span>](#property-get_property_translation_key) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `property`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_set_glossary_entry_translation_id</span>](#property-get_set_glossary_entry_translation_id) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_set_glossary_translation_id</span>](#property-get_set_glossary_translation_id) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_set_regex_option</span>](#property-get_set_regex_option) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_word_translation_key</span>](#property-get_word_translation_key) ( `word`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">remove_entry</span>](#property-remove_entry) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">remove_entry_translation_ids</span>](#property-remove_entry_translation_ids) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">remove_translation_id</span>](#property-remove_translation_id) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">replace_entry_key</span>](#property-replace_entry_key) ( `old_entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">try_add_entry</span>](#property-try_add_entry) ( `entry`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
--- 
## Constants


<a class="header" id="constant-RESOURCE_NAME" href="#constant-RESOURCE_NAME">**<span class="hljs-attribute">const</span> <span class="hljs-title">RESOURCE_NAME</span><span class="hljs-comment"> = "Glossary"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-NAME_PROPERTY" href="#constant-NAME_PROPERTY">**<span class="hljs-attribute">const</span> <span class="hljs-title">NAME_PROPERTY</span><span class="hljs-comment"> = "name"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ALTERNATIVE_PROPERTY" href="#constant-ALTERNATIVE_PROPERTY">**<span class="hljs-attribute">const</span> <span class="hljs-title">ALTERNATIVE_PROPERTY</span><span class="hljs-comment"> = "alternatives"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TITLE_PROPERTY" href="#constant-TITLE_PROPERTY">**<span class="hljs-attribute">const</span> <span class="hljs-title">TITLE_PROPERTY</span><span class="hljs-comment"> = "title"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TEXT_PROPERTY" href="#constant-TEXT_PROPERTY">**<span class="hljs-attribute">const</span> <span class="hljs-title">TEXT_PROPERTY</span><span class="hljs-comment"> = "text"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-EXTRA_PROPERTY" href="#constant-EXTRA_PROPERTY">**<span class="hljs-attribute">const</span> <span class="hljs-title">EXTRA_PROPERTY</span><span class="hljs-comment"> = "extra"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TRANSLATION_PROPERTY" href="#constant-TRANSLATION_PROPERTY">**<span class="hljs-attribute">const</span> <span class="hljs-title">TRANSLATION_PROPERTY</span><span class="hljs-comment"> = "_translation_id"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-REGEX_OPTION_PROPERTY" href="#constant-REGEX_OPTION_PROPERTY">**<span class="hljs-attribute">const</span> <span class="hljs-title">REGEX_OPTION_PROPERTY</span><span class="hljs-comment"> = "regex_options"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-PRIVATE_PROPERTY_PREFIX" href="#constant-PRIVATE_PROPERTY_PREFIX">**<span class="hljs-attribute">const</span> <span class="hljs-title">PRIVATE_PROPERTY_PREFIX</span><span class="hljs-comment"> = "_"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-_MISSING_ENTRY_INDEX" href="#constant-_MISSING_ENTRY_INDEX">**<span class="hljs-attribute">const</span> <span class="hljs-title">_MISSING_ENTRY_INDEX</span><span class="hljs-comment"> = -1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-add_translation_id" href="#property-add_translation_id">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_translation_id</span>](#property-add_translation_id) ( )** </a>



This is automatically called, no need to use this.

---



<a class="header" id="property-clear_translation_keys" href="#property-clear_translation_keys">**<span class="hljs-attribute">void</span> [<span class="hljs-title">clear_translation_keys</span>](#property-clear_translation_keys) ( )** </a>



Clears the lookup tables using translation keys.

---



<a class="header" id="property-get_entry" href="#property-get_entry">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_entry</span>](#property-get_entry) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



Gets the glossary entry for the given `entry_key`. If there is no matching entry, an empty Dictionary will be returned. Valid glossary entry dictionaries will never be empty.

---



<a class="header" id="property-get_property_translation_key" href="#property-get_property_translation_key">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_property_translation_key</span>](#property-get_property_translation_key) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `property`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



Returns a key used to reference this glossary in the translation CSV file.  Time complexity: O(1)

---



<a class="header" id="property-get_set_glossary_entry_translation_id" href="#property-get_set_glossary_entry_translation_id">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_set_glossary_entry_translation_id</span>](#property-get_set_glossary_entry_translation_id) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



Tries to get the glossary entry's translation ID. If it does not exist, a new one will be generated.

---



<a class="header" id="property-get_set_glossary_translation_id" href="#property-get_set_glossary_translation_id">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_set_glossary_translation_id</span>](#property-get_set_glossary_translation_id) ( )** </a>



Tries to get the glossary's translation ID. If it does not exist, a new one will be generated.

---



<a class="header" id="property-get_set_regex_option" href="#property-get_set_regex_option">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_set_regex_option</span>](#property-get_set_regex_option) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



Gets the regex option for the given `entry_key`. If the regex option does not exist, it will be generated.  A regex option is the accumulation of valid words that can trigger the glossary popup.  The `entry_key` must be valid or an error will occur.

---



<a class="header" id="property-get_word_translation_key" href="#property-get_word_translation_key">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_word_translation_key</span>](#property-get_word_translation_key) ( `word`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



Returns the matching translation key for the given `word`. This key can be used via [tr](#property-tr) to get the translation.  Time complexity: O(1) Uses an internal dictionary to find the translation key. This dictionary is generated when the glossary is translated. See `_translation_keys`.

---



<a class="header" id="property-remove_entry" href="#property-remove_entry">**<span class="hljs-attribute">void</span> [<span class="hljs-title">remove_entry</span>](#property-remove_entry) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



Removes an entry and all its aliases (alternative property) from the glossary. `entry_key` may be an entry name or an alias.  Returns true if the entry matching the given `entry_key` was found.

---



<a class="header" id="property-remove_entry_translation_ids" href="#property-remove_entry_translation_ids">**<span class="hljs-attribute">void</span> [<span class="hljs-title">remove_entry_translation_ids</span>](#property-remove_entry_translation_ids) ( )** </a>



Removes the translation ID of all glossary entries.

---



<a class="header" id="property-remove_translation_id" href="#property-remove_translation_id">**<span class="hljs-attribute">void</span> [<span class="hljs-title">remove_translation_id</span>](#property-remove_translation_id) ( )** </a>



Removes the translation ID of this glossary.

---



<a class="header" id="property-replace_entry_key" href="#property-replace_entry_key">**<span class="hljs-attribute">void</span> [<span class="hljs-title">replace_entry_key</span>](#property-replace_entry_key) ( `old_entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



Do not use this to update alternative names. In order to update alternative names, delete all with `_remove_entry_alias` and then add them again with `_add_entry_key_alias`.

---



<a class="header" id="property-try_add_entry" href="#property-try_add_entry">**<span class="hljs-attribute">void</span> [<span class="hljs-title">try_add_entry</span>](#property-try_add_entry) ( `entry`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



Adds `entry` to the glossary if it does not exist. If it does exist, returns false.

---

