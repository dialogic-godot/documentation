
<div class="header-banner purple">
<div class="header-label purple">DialogicResourceUtil</div>
</div>

*This contains the source code documentation of the class `DialogicResourceUtil`.*
        
# DialogicResourceUtil
**Inherits:** RefCounted

##############################################################################
## Properties
Name | Type | Default 
--- | --- | --- 
event_cache | [DialogicEvent[]](https://docs.godotengine.org/en/latest/classes/class_dialogicevent.html#class-dialogicevent) |   
label_cache | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
special_resources | [Dictionary[]](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_resource_to_directory</span>](#property-add_resource_to_directory) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `directory`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">change_resource_path</span>](#property-change_resource_path) ( `old_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">change_unique_identifier</span>](#property-change_unique_identifier) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_character_directory</span>](#property-get_character_directory) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_character_resource</span>](#property-get_character_resource) ( `character_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_directory</span>](#property-get_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_event_cache</span>](#property-get_event_cache) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_label_cache</span>](#property-get_label_cache) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_resource_from_identifier</span>](#property-get_resource_from_identifier) ( `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_timeline_directory</span>](#property-get_timeline_directory) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_timeline_resource</span>](#property-get_timeline_resource) ( `timeline_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_unique_identifier</span>](#property-get_unique_identifier) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">guess_special_resource</span>](#property-guess_special_resource) ( `type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">is_identifier_unused</span>](#property-is_identifier_unused) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">list_resources_of_type</span>](#property-list_resources_of_type) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">list_special_resources_of_type</span>](#property-list_special_resources_of_type) ( `type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">remove_resource</span>](#property-remove_resource) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">scan_folder</span>](#property-scan_folder) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">set_directory</span>](#property-set_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `directory`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">set_label_cache</span>](#property-set_label_cache) ( `cache`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">update</span>](#property-update) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">update_directory</span>](#property-update_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">update_event_cache</span>](#property-update_event_cache) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">update_label_cache</span>](#property-update_label_cache) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">update_special_resources</span>](#property-update_special_resources) ( ) 
--- 
## Property Descriptions



<a class="header" id="property-add_resource_to_directory" href="#property-add_resource_to_directory">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_resource_to_directory</span>](#property-add_resource_to_directory) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `directory`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-change_resource_path" href="#property-change_resource_path">**<span class="hljs-attribute">void</span> [<span class="hljs-title">change_resource_path</span>](#property-change_resource_path) ( `old_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-change_unique_identifier" href="#property-change_unique_identifier">**<span class="hljs-attribute">void</span> [<span class="hljs-title">change_unique_identifier</span>](#property-change_unique_identifier) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_character_directory" href="#property-get_character_directory">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_character_directory</span>](#property-get_character_directory) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_character_resource" href="#property-get_character_resource">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_character_resource</span>](#property-get_character_resource) ( `character_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_directory" href="#property-get_directory">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_directory</span>](#property-get_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_event_cache" href="#property-get_event_cache">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_event_cache</span>](#property-get_event_cache) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_label_cache" href="#property-get_label_cache">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_label_cache</span>](#property-get_label_cache) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_resource_from_identifier" href="#property-get_resource_from_identifier">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_resource_from_identifier</span>](#property-get_resource_from_identifier) ( `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_timeline_directory" href="#property-get_timeline_directory">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_timeline_directory</span>](#property-get_timeline_directory) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_timeline_resource" href="#property-get_timeline_resource">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_timeline_resource</span>](#property-get_timeline_resource) ( `timeline_identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_unique_identifier" href="#property-get_unique_identifier">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_unique_identifier</span>](#property-get_unique_identifier) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-guess_special_resource" href="#property-guess_special_resource">**<span class="hljs-attribute">void</span> [<span class="hljs-title">guess_special_resource</span>](#property-guess_special_resource) ( `type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_identifier_unused" href="#property-is_identifier_unused">**<span class="hljs-attribute">void</span> [<span class="hljs-title">is_identifier_unused</span>](#property-is_identifier_unused) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `identifier`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-list_resources_of_type" href="#property-list_resources_of_type">**<span class="hljs-attribute">void</span> [<span class="hljs-title">list_resources_of_type</span>](#property-list_resources_of_type) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-list_special_resources_of_type" href="#property-list_special_resources_of_type">**<span class="hljs-attribute">void</span> [<span class="hljs-title">list_special_resources_of_type</span>](#property-list_special_resources_of_type) ( `type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-remove_resource" href="#property-remove_resource">**<span class="hljs-attribute">void</span> [<span class="hljs-title">remove_resource</span>](#property-remove_resource) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-scan_folder" href="#property-scan_folder">**<span class="hljs-attribute">void</span> [<span class="hljs-title">scan_folder</span>](#property-scan_folder) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_directory" href="#property-set_directory">**<span class="hljs-attribute">void</span> [<span class="hljs-title">set_directory</span>](#property-set_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `directory`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_label_cache" href="#property-set_label_cache">**<span class="hljs-attribute">void</span> [<span class="hljs-title">set_label_cache</span>](#property-set_label_cache) ( `cache`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-update" href="#property-update">**<span class="hljs-attribute">void</span> [<span class="hljs-title">update</span>](#property-update) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-update_directory" href="#property-update_directory">**<span class="hljs-attribute">void</span> [<span class="hljs-title">update_directory</span>](#property-update_directory) ( `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-update_event_cache" href="#property-update_event_cache">**<span class="hljs-attribute">void</span> [<span class="hljs-title">update_event_cache</span>](#property-update_event_cache) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-update_label_cache" href="#property-update_label_cache">**<span class="hljs-attribute">void</span> [<span class="hljs-title">update_label_cache</span>](#property-update_label_cache) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-update_special_resources" href="#property-update_special_resources">**<span class="hljs-attribute">void</span> [<span class="hljs-title">update_special_resources</span>](#property-update_special_resources) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

