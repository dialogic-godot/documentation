
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
[<span class="hljs-title">add_separator</span>](#property-add_separator) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">column_count</span>](#property-column_count) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">file</span>](#property-file) | [FileAccess](https://docs.godotengine.org/en/latest/classes/class_fileaccess.html#class-fileaccess) |   
[<span class="hljs-title">is_new_file</span>](#property-is_new_file) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">lines</span>](#property-lines) | [PackedStringArray[]](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray) |   
[<span class="hljs-title">new_rows</span>](#property-new_rows) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">old_lines</span>](#property-old_lines) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">updated_rows</span>](#property-updated_rows) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">used_file_path</span>](#property-used_file_path) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_translation_keys_to_glossary</span>](#method-add_translation_keys_to_glossary) ( `glossary`: [DialogicGlossary](class_dialogicglossary.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">collect_lines_from_characters</span>](#method-collect_lines_from_characters) ( `characters`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">collect_lines_from_glossary</span>](#method-collect_lines_from_glossary) ( `glossary`: [DialogicGlossary](class_dialogicglossary.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">collect_lines_from_timeline</span>](#method-collect_lines_from_timeline) ( `timeline`: [DialogicTimeline](class_dialogictimeline.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_csv_file_on_disk</span>](#method-update_csv_file_on_disk) ( ) 
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



<a class="header" id="property-add_separator" href="#property-add_separator">**<span class="hljs-attribute">var</span> <span class="hljs-title">add_separator</span> <span style = "color: gray"> = </span> false** 



Whether this CSV handler should add newlines as a separator between sections. A section may be a new character, new timeline, or new glossary item inside a per-project file.

---



<a class="header" id="property-column_count" href="#property-column_count">**<span class="hljs-attribute">var</span> <span class="hljs-title">column_count</span> <span style = "color: gray"> = </span> 0** 



The amount of columns the CSV file has after loading it. Used to add trailing commas to new lines.

---



<a class="header" id="property-file" href="#property-file">**<span class="hljs-attribute">var</span> <span class="hljs-title">file</span>** 



The underlying file used to read and write the CSV file.

---



<a class="header" id="property-is_new_file" href="#property-is_new_file">**<span class="hljs-attribute">var</span> <span class="hljs-title">is_new_file</span> <span style = "color: gray"> = </span> false** 



Whether this CSV file was able to be loaded a defined file path.

---



<a class="header" id="property-lines" href="#property-lines">**<span class="hljs-attribute">var</span> <span class="hljs-title">lines</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-new_rows" href="#property-new_rows">**<span class="hljs-attribute">var</span> <span class="hljs-title">new_rows</span> <span style = "color: gray"> = </span> 0** 



The amount of events that were added to the CSV file.

---



<a class="header" id="property-old_lines" href="#property-old_lines">**<span class="hljs-attribute">var</span> <span class="hljs-title">old_lines</span> <span style = "color: gray"> = </span> <unknown>** 



Dictionary of lines from the original file. Key: String, Value: PackedStringArray

---



<a class="header" id="property-updated_rows" href="#property-updated_rows">**<span class="hljs-attribute">var</span> <span class="hljs-title">updated_rows</span> <span style = "color: gray"> = </span> 0** 



The amount of events that were updated in the CSV file.

---



<a class="header" id="property-used_file_path" href="#property-used_file_path">**<span class="hljs-attribute">var</span> <span class="hljs-title">used_file_path</span>** 



File path used to load the CSV file.

---

## Method Descriptions



<a class="header" id="method-add_translation_keys_to_glossary" href="#method-add_translation_keys_to_glossary">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_translation_keys_to_glossary</span>](#method-add_translation_keys_to_glossary) ( `glossary`: [DialogicGlossary](class_dialogicglossary.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Reads all `lines` and adds them to the given `glossary`'s internal collection of words-to-translation-key mappings.  Populate the CSV's lines with the method [collect_lines_from_glossary](#property-collect_lines_from_glossary) before.

---



<a class="header" id="method-collect_lines_from_characters" href="#method-collect_lines_from_characters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">collect_lines_from_characters</span>](#method-collect_lines_from_characters) ( `characters`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span style = "color: gray">void</span>** 



Collects names from the given `characters` and adds them to the `lines`.  If this is the character name CSV file, use this method to take previously collected characters from other [DialogicCsvFile](class_dialogiccsvfile.md)s.

---



<a class="header" id="method-collect_lines_from_glossary" href="#method-collect_lines_from_glossary">**<span class="hljs-attribute">func</span> [<span class="hljs-title">collect_lines_from_glossary</span>](#method-collect_lines_from_glossary) ( `glossary`: [DialogicGlossary](class_dialogicglossary.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Collects properties from glossary entries from the given `glossary` and adds them to the `lines`.

---



<a class="header" id="method-collect_lines_from_timeline" href="#method-collect_lines_from_timeline">**<span class="hljs-attribute">func</span> [<span class="hljs-title">collect_lines_from_timeline</span>](#method-collect_lines_from_timeline) ( `timeline`: [DialogicTimeline](class_dialogictimeline.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Collects translatable events from the given `timeline` and adds them to the `lines`.

---



<a class="header" id="method-update_csv_file_on_disk" href="#method-update_csv_file_on_disk">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_csv_file_on_disk</span>](#method-update_csv_file_on_disk) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Clears the CSV file on disk and writes the current `lines` array to it. Uses the `old_lines` dictionary to update existing translations. If a translation row misses a column, a trailing comma will be added to conform to the CSV file format.  If the locale CSV line was collected only, a new file won't be created and already existing translations won't be updated.

---

