
<div class="header-banner purple">
<div class="header-label purple">DialogicResourceUtil</div>
</div>

*This contains the source code documentation of the class `DialogicResourceUtil`.*
        
# DialogicResourceUtil
**Inherits:** [RefCounted](https://docs.godotengine.org/en/latest/classes/class_refcounted.html#class-refcounted)


## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">label_cache</span>](#property-label_cache) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{}` 
[<span class="hljs-title">event_cache</span>](#property-event_cache) | [DialogicEvent[]](https://docs.godotengine.org/en/latest/classes/class_dialogicevent.html#class-dialogicevent) |  `[]` 
[<span class="hljs-title">channel_cache</span>](#property-channel_cache) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{}` 
[<span class="hljs-title">special_resources</span>](#property-special_resources) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{}` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">update</span>](#method-update) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_directory</span>](#method-get_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_directory</span>](#method-set_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `directory`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_directory</span>](#method-update_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">add_resource_to_directory</span>](#method-add_resource_to_directory) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `directory`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_unique_identifier_by_path</span>](#method-get_unique_identifier_by_path) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_resource_path_from_identifier</span>](#method-get_resource_path_from_identifier) ( `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource)</span> | [<span class="hljs-title">get_resource_from_identifier</span>](#method-get_resource_from_identifier) ( `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">resource_exists_from_identifier</span>](#method-resource_exists_from_identifier) ( `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_unique_identifier</span>](#method-change_unique_identifier) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_resource_path</span>](#method-change_resource_path) ( `old_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">remove_resource</span>](#method-remove_resource) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_identifier_unused</span>](#method-is_identifier_unused) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">register_runtime_resource</span>](#method-register_runtime_resource) ( `resource`: [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource), `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_runtime_unique_identifier</span>](#method-get_runtime_unique_identifier) ( `resource`: [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_label_cache</span>](#method-get_label_cache) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_label_cache</span>](#method-set_label_cache) ( `cache`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_label_cache</span>](#method-update_label_cache) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_audio_channel_cache</span>](#method-get_audio_channel_cache) ( ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_channel_list</span>](#method-get_channel_list) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_audio_channel_cache</span>](#method-set_audio_channel_cache) ( `cache`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_audio_channel_cache</span>](#method-update_audio_channel_cache) ( ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_event_cache</span>](#method-get_event_cache) ( ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">update_event_cache</span>](#method-update_event_cache) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_special_resources</span>](#method-update_special_resources) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">list_special_resources</span>](#method-list_special_resources) ( `type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `filter`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">match_resource_filter</span>](#method-match_resource_filter) ( `dict`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `filter`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">guess_special_resource</span>](#method-guess_special_resource) ( `type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}`, `filter`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}`, `ignores`: [PackedStringArray](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray) = `[]` ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_character_directory</span>](#method-get_character_directory) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_timeline_directory</span>](#method-get_timeline_directory) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">timeline_resource_exists</span>](#method-timeline_resource_exists) ( `timeline_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[DialogicTimeline](class_dialogictimeline.md)</span> | [<span class="hljs-title">get_timeline_resource</span>](#method-get_timeline_resource) ( `timeline_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[DialogicCharacter](class_dialogiccharacter.md)</span> | [<span class="hljs-title">get_character_resource</span>](#method-get_character_resource) ( `character_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">list_resources_of_type</span>](#method-list_resources_of_type) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">scan_folder</span>](#method-scan_folder) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
--- 
## Property Descriptions



<a class="header" id="property-label_cache" href="#property-label_cache">**<span class="hljs-attribute">var</span> <span class="hljs-title">label_cache</span> <span style = "color: gray"> = </span> {}** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-event_cache" href="#property-event_cache">**<span class="hljs-attribute">var</span> <span class="hljs-title">event_cache</span> <span style = "color: gray"> = </span> []** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-channel_cache" href="#property-channel_cache">**<span class="hljs-attribute">var</span> <span class="hljs-title">channel_cache</span> <span style = "color: gray"> = </span> {}** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-special_resources" href="#property-special_resources">**<span class="hljs-attribute">var</span> <span class="hljs-title">special_resources</span> <span style = "color: gray"> = </span> {}** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-update" href="#method-update">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update</span>](#method-update) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_directory" href="#method-get_directory">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_directory</span>](#method-get_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_directory" href="#method-set_directory">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_directory</span>](#method-set_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `directory`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_directory" href="#method-update_directory">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_directory</span>](#method-update_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-add_resource_to_directory" href="#method-add_resource_to_directory">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_resource_to_directory</span>](#method-add_resource_to_directory) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `directory`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_unique_identifier_by_path" href="#method-get_unique_identifier_by_path">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_unique_identifier_by_path</span>](#method-get_unique_identifier_by_path) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the unique identifier for the given resource path. Returns an empty string if no identifier was found.

---



<a class="header" id="method-get_resource_path_from_identifier" href="#method-get_resource_path_from_identifier">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_resource_path_from_identifier</span>](#method-get_resource_path_from_identifier) ( `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_resource_from_identifier" href="#method-get_resource_from_identifier">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_resource_from_identifier</span>](#method-get_resource_from_identifier) ( `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource)</span>** 



Returns the resource associated with the given unique identifier. The expected extension is needed to use the right directory.

---



<a class="header" id="method-resource_exists_from_identifier" href="#method-resource_exists_from_identifier">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resource_exists_from_identifier</span>](#method-resource_exists_from_identifier) ( `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns a boolean that expresses whether the resource exists. The expected extension is needed to use the right directory.

---



<a class="header" id="method-change_unique_identifier" href="#method-change_unique_identifier">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_unique_identifier</span>](#method-change_unique_identifier) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Editor Only

---



<a class="header" id="method-change_resource_path" href="#method-change_resource_path">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_resource_path</span>](#method-change_resource_path) ( `old_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-remove_resource" href="#method-remove_resource">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_resource</span>](#method-remove_resource) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_identifier_unused" href="#method-is_identifier_unused">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_identifier_unused</span>](#method-is_identifier_unused) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-register_runtime_resource" href="#method-register_runtime_resource">**<span class="hljs-attribute">func</span> [<span class="hljs-title">register_runtime_resource</span>](#method-register_runtime_resource) ( `resource`: [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource), `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



While usually the directory maps identifiers to paths, this method (only supposed to be used at runtime) allows mapping resources that are not saved to an identifier.

---



<a class="header" id="method-get_runtime_unique_identifier" href="#method-get_runtime_unique_identifier">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_runtime_unique_identifier</span>](#method-get_runtime_unique_identifier) ( `resource`: [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_label_cache" href="#method-get_label_cache">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_label_cache</span>](#method-get_label_cache) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_label_cache" href="#method-set_label_cache">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_label_cache</span>](#method-set_label_cache) ( `cache`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_label_cache" href="#method-update_label_cache">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_label_cache</span>](#method-update_label_cache) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_audio_channel_cache" href="#method-get_audio_channel_cache">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_audio_channel_cache</span>](#method-get_audio_channel_cache) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_channel_list" href="#method-get_channel_list">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_channel_list</span>](#method-get_channel_list) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_audio_channel_cache" href="#method-set_audio_channel_cache">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_audio_channel_cache</span>](#method-set_audio_channel_cache) ( `cache`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_audio_channel_cache" href="#method-update_audio_channel_cache">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_audio_channel_cache</span>](#method-update_audio_channel_cache) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_event_cache" href="#method-get_event_cache">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_event_cache</span>](#method-get_event_cache) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



Dialogic keeps a list that has each event once. This allows retrieval of that list.

---



<a class="header" id="method-update_event_cache" href="#method-update_event_cache">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_event_cache</span>](#method-update_event_cache) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_special_resources" href="#method-update_special_resources">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_special_resources</span>](#method-update_special_resources) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-list_special_resources" href="#method-list_special_resources">**<span class="hljs-attribute">func</span> [<span class="hljs-title">list_special_resources</span>](#method-list_special_resources) ( `type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `filter`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-match_resource_filter" href="#method-match_resource_filter">**<span class="hljs-attribute">func</span> [<span class="hljs-title">match_resource_filter</span>](#method-match_resource_filter) ( `dict`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `filter`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-guess_special_resource" href="#method-guess_special_resource">**<span class="hljs-attribute">func</span> [<span class="hljs-title">guess_special_resource</span>](#method-guess_special_resource) ( `type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}`, `filter`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}`, `ignores`: [PackedStringArray](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray) = `[]` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_character_directory" href="#method-get_character_directory">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_directory</span>](#method-get_character_directory) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_timeline_directory" href="#method-get_timeline_directory">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_timeline_directory</span>](#method-get_timeline_directory) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-timeline_resource_exists" href="#method-timeline_resource_exists">**<span class="hljs-attribute">func</span> [<span class="hljs-title">timeline_resource_exists</span>](#method-timeline_resource_exists) ( `timeline_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_timeline_resource" href="#method-get_timeline_resource">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_timeline_resource</span>](#method-get_timeline_resource) ( `timeline_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[DialogicTimeline](class_dialogictimeline.md)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_character_resource" href="#method-get_character_resource">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_resource</span>](#method-get_character_resource) ( `character_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[DialogicCharacter](class_dialogiccharacter.md)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-list_resources_of_type" href="#method-list_resources_of_type">**<span class="hljs-attribute">func</span> [<span class="hljs-title">list_resources_of_type</span>](#method-list_resources_of_type) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-scan_folder" href="#method-scan_folder">**<span class="hljs-attribute">func</span> [<span class="hljs-title">scan_folder</span>](#method-scan_folder) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

