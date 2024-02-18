
<div class="header-banner purple">
<div class="header-label purple">DialogicIndexer</div>
</div>

*This contains the source code documentation of the class `DialogicIndexer`.*
        
# DialogicIndexer
**Inherits:** [RefCounted](https://docs.godotengine.org/en/latest/classes/class_refcounted.html#class-refcounted)

Script that indexes events, subsystems, settings pages and more. [br]Place a script of this type in every folder in "addons/Events". [br]Overwrite the methods to return the contents of that folder.
## Properties
Name | Type | Default 
--- | --- | --- 
this_folder | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">list_dir</span>](#property-list_dir) ( `subdir`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[Dictionary[]](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">list_special_resources</span>](#property-list_special_resources) ( `subdir`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[Dictionary[]](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">scan_for_layout_parts</span>](#property-scan_for_layout_parts) ( ) 
--- 
## Property Descriptions



<a class="header" id="property-list_dir" href="#property-list_dir">**<span class="hljs-attribute">func</span> [<span class="hljs-title">list_dir</span>](#property-list_dir) ( `subdir`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-list_special_resources" href="#property-list_special_resources">**<span class="hljs-attribute">func</span> [<span class="hljs-title">list_special_resources</span>](#property-list_special_resources) ( `subdir`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `extension`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary[]](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-scan_for_layout_parts" href="#property-scan_for_layout_parts">**<span class="hljs-attribute">func</span> [<span class="hljs-title">scan_for_layout_parts</span>](#property-scan_for_layout_parts) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary[]](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Helper that allows scanning sub directories that might be layout parts or styles

---

