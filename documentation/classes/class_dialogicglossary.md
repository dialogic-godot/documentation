
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
[<span class="hljs-title">entries</span>](#property-entries) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{}` 
[<span class="hljs-title">enabled</span>](#property-enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">remove_entry</span>](#method-remove_entry) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">replace_entry_key</span>](#method-replace_entry_key) ( `old_entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_entry</span>](#method-get_entry) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">try_add_entry</span>](#method-try_add_entry) ( `entry`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_set_regex_option</span>](#method-get_set_regex_option) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">add_translation_id</span>](#method-add_translation_id) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">remove_translation_id</span>](#method-remove_translation_id) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">remove_entry_translation_ids</span>](#method-remove_entry_translation_ids) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_translation_keys</span>](#method-clear_translation_keys) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_property_translation_key</span>](#method-get_property_translation_key) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `property`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_set_glossary_entry_translation_id</span>](#method-get_set_glossary_entry_translation_id) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_set_glossary_translation_id</span>](#method-get_set_glossary_translation_id) ( ) 
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
## Property Descriptions



<a class="header" id="property-entries" href="#property-entries">**<span class="hljs-attribute">var</span> <span class="hljs-title">entries</span> <span style = "color: gray"> = </span> {}** 



Stores all entries for the glossary.  The value may either be a dictionary, representing an entry, or a string, representing the actual key for the key used. The string key-value pairs are the alias keys, they allow to redirect the actual glossary entry.

---



<a class="header" id="property-enabled" href="#property-enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">enabled</span> <span style = "color: gray"> = </span> true** 



If false, no entries from this glossary will be shown

---

## Method Descriptions



<a class="header" id="method-remove_entry" href="#method-remove_entry">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_entry</span>](#method-remove_entry) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Removes an entry and all its aliases (alternative property) from the glossary. `entry_key` may be an entry name or an alias.  Returns true if the entry matching the given `entry_key` was found.

---



<a class="header" id="method-replace_entry_key" href="#method-replace_entry_key">**<span class="hljs-attribute">func</span> [<span class="hljs-title">replace_entry_key</span>](#method-replace_entry_key) ( `old_entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Do not use this to update alternative names. In order to update alternative names, delete all with `_remove_entry_alias` and then add them again with `_add_entry_key_alias`.

---



<a class="header" id="method-get_entry" href="#method-get_entry">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_entry</span>](#method-get_entry) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Gets the glossary entry for the given `entry_key`. If there is no matching entry, an empty Dictionary will be returned. Valid glossary entry dictionaries will never be empty.

---



<a class="header" id="method-try_add_entry" href="#method-try_add_entry">**<span class="hljs-attribute">func</span> [<span class="hljs-title">try_add_entry</span>](#method-try_add_entry) ( `entry`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Adds `entry` to the glossary if it does not exist. If it does exist, returns false.

---



<a class="header" id="method-get_set_regex_option" href="#method-get_set_regex_option">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_set_regex_option</span>](#method-get_set_regex_option) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Gets the regex option for the given `entry_key`. If the regex option does not exist, it will be generated.  A regex option is the accumulation of valid words that can trigger the glossary popup.  The `entry_key` must be valid or an error will occur.

---



<a class="header" id="method-add_translation_id" href="#method-add_translation_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_translation_id</span>](#method-add_translation_id) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



This is automatically called, no need to use this.

---



<a class="header" id="method-remove_translation_id" href="#method-remove_translation_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_translation_id</span>](#method-remove_translation_id) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Removes the translation ID of this glossary.

---



<a class="header" id="method-remove_entry_translation_ids" href="#method-remove_entry_translation_ids">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_entry_translation_ids</span>](#method-remove_entry_translation_ids) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Removes the translation ID of all glossary entries.

---



<a class="header" id="method-clear_translation_keys" href="#method-clear_translation_keys">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_translation_keys</span>](#method-clear_translation_keys) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Clears the lookup tables using translation keys.

---



<a class="header" id="method-get_property_translation_key" href="#method-get_property_translation_key">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_property_translation_key</span>](#method-get_property_translation_key) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `property`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns a key used to reference this glossary in the translation CSV file.  Time complexity: O(1)

---



<a class="header" id="method-get_set_glossary_entry_translation_id" href="#method-get_set_glossary_entry_translation_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_set_glossary_entry_translation_id</span>](#method-get_set_glossary_entry_translation_id) ( `entry_key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Tries to get the glossary entry's translation ID. If it does not exist, a new one will be generated.

---



<a class="header" id="method-get_set_glossary_translation_id" href="#method-get_set_glossary_translation_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_set_glossary_translation_id</span>](#method-get_set_glossary_translation_id) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Tries to get the glossary's translation ID. If it does not exist, a new one will be generated.

---

