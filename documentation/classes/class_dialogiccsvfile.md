
<div class="header-banner purple">
<div class="header-label purple">DialogicCsvFile</div>
</div>

*This contains the source code documentation of the class `DialogicCsvFile`.*
        
# DialogicCsvFile
**Inherits:** [RefCounted](https://docs.godotengine.org/en/latest/classes/class_refcounted.html#class-refcounted)

Handles translation of a [DialogicTimeline](class_dialogictimeline.md) to a CSV file.
## Properties
Name | Type | Default 
--- | --- | --- 
add_separator | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
column_count | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
file | [FileAccess](https://docs.godotengine.org/en/latest/classes/class_fileaccess.html#class-fileaccess) |   
is_new_file | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
lines | [PackedStringArray[]](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray) |   
new_rows | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
old_lines | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
updated_rows | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
used_file_path | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_translation_keys_to_glossary</span>](#property-add_translation_keys_to_glossary) ( `glossary`: [DialogicGlossary](class_dialogicglossary.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">collect_lines_from_characters</span>](#property-collect_lines_from_characters) ( `characters`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">collect_lines_from_glossary</span>](#property-collect_lines_from_glossary) ( `glossary`: [DialogicGlossary](class_dialogicglossary.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">collect_lines_from_timeline</span>](#property-collect_lines_from_timeline) ( `timeline`: [DialogicTimeline](class_dialogictimeline.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_csv_file_on_disk</span>](#property-update_csv_file_on_disk) ( ) 
--- 
## Constants


<a class="header" id="constant-String" href="#constant-String">**<span class="hljs-attribute">const</span> <span class="hljs-title">String</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-Array" href="#constant-Array">**<span class="hljs-attribute">const</span> <span class="hljs-title">Array</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-Other" href="#constant-Other">**<span class="hljs-attribute">const</span> <span class="hljs-title">Other</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TRANSLATION_ID" href="#constant-TRANSLATION_ID">**<span class="hljs-attribute">const</span> <span class="hljs-title">TRANSLATION_ID</span><span class="hljs-comment"> = "_translation_id"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-add_translation_keys_to_glossary" href="#property-add_translation_keys_to_glossary">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_translation_keys_to_glossary</span>](#property-add_translation_keys_to_glossary) ( `glossary`: [DialogicGlossary](class_dialogicglossary.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Reads all `lines` and adds them to the given `glossary`'s internal collection of words-to-translation-key mappings.  Populate the CSV's lines with the method [collect_lines_from_glossary](#property-collect_lines_from_glossary) before.

---



<a class="header" id="property-collect_lines_from_characters" href="#property-collect_lines_from_characters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">collect_lines_from_characters</span>](#property-collect_lines_from_characters) ( `characters`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span style = "color: gray">void</span>** 



Collects names from the given `characters` and adds them to the `lines`.  If this is the character name CSV file, use this method to take previously collected characters from other [DialogicCsvFile](class_dialogiccsvfile.md)s.

---



<a class="header" id="property-collect_lines_from_glossary" href="#property-collect_lines_from_glossary">**<span class="hljs-attribute">func</span> [<span class="hljs-title">collect_lines_from_glossary</span>](#property-collect_lines_from_glossary) ( `glossary`: [DialogicGlossary](class_dialogicglossary.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Collects properties from glossary entries from the given `glossary` and adds them to the `lines`.

---



<a class="header" id="property-collect_lines_from_timeline" href="#property-collect_lines_from_timeline">**<span class="hljs-attribute">func</span> [<span class="hljs-title">collect_lines_from_timeline</span>](#property-collect_lines_from_timeline) ( `timeline`: [DialogicTimeline](class_dialogictimeline.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Collects translatable events from the given `timeline` and adds them to the `lines`.

---



<a class="header" id="property-update_csv_file_on_disk" href="#property-update_csv_file_on_disk">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_csv_file_on_disk</span>](#property-update_csv_file_on_disk) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Clears the CSV file on disk and writes the current `lines` array to it. Uses the `old_lines` dictionary to update existing translations. If a translation row misses a column, a trailing comma will be added to conform to the CSV file format.  If the locale CSV line was collected only, a new file won't be created and already existing translations won't be updated.

---

