
<div class="header-banner purple">
<div class="header-label purple">DialogicSidebar</div>
</div>

*This contains the source code documentation of the class `DialogicSidebar`.*
        
# DialogicSidebar
**Inherits:** [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)

############################################################################## RESOURCE LIST ##############################################################################
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">editors_manager</span>](#property-editors_manager) | [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) |  `get_parent()` 
[<span class="hljs-title">resource_tree</span>](#property-resource_tree) | [Tree](https://docs.godotengine.org/en/latest/classes/class_tree.html#class-tree) |   
[<span class="hljs-title">current_resource_list</span>](#property-current_resource_list) | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |  `[]` 
[<span class="hljs-title">sort_mode</span>](#property-sort_mode) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[PackedStringArray](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray)</span> | [<span class="hljs-title">clean_resource_list</span>](#method-clean_resource_list) ( `resources_list`: [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) = `[]` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_resource_list</span>](#method-update_resource_list) ( `resources_list`: [PackedStringArray](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray) = `[]` ) 
<span class="hljs-attribute">[TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem)</span> | [<span class="hljs-title">add_item</span>](#method-add_item) ( `item`: [DialogicSidebar.ResourceListItem](class_dialogicsidebar.resourcelistitem.md), `parent`: [TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem), `current_file`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem)</span> | [<span class="hljs-title">add_folder_item</span>](#method-add_folder_item) ( `label`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `parent`: [TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_unsaved_indicator</span>](#method-set_unsaved_indicator) ( `saved`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_content_list</span>](#method-update_content_list) ( `list`: [PackedStringArray](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">remove_item_from_list</span>](#method-remove_item_from_list) ( `item`: [TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">edit_resource</span>](#method-edit_resource) ( `resource_item`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
--- 
## Constants


<a class="header" id="constant-TYPE" href="#constant-TYPE">**<span class="hljs-attribute">const</span> <span class="hljs-title">TYPE</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-FOLDER" href="#constant-FOLDER">**<span class="hljs-attribute">const</span> <span class="hljs-title">FOLDER</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-PATH" href="#constant-PATH">**<span class="hljs-attribute">const</span> <span class="hljs-title">PATH</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-NONE" href="#constant-NONE">**<span class="hljs-attribute">const</span> <span class="hljs-title">NONE</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-file_activated" href="#signal-file_activated">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">file_activated</span>](#signal-file_activated) ( `file_path`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-content_item_activated" href="#signal-content_item_activated">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">content_item_activated</span>](#signal-content_item_activated) ( `item_name`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-show_sidebar" href="#signal-show_sidebar">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">show_sidebar</span>](#signal-show_sidebar) ( `show`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-editors_manager" href="#property-editors_manager">**<span class="hljs-attribute">var</span> <span class="hljs-title">editors_manager</span> <span style = "color: gray"> = </span> get_parent()** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-resource_tree" href="#property-resource_tree">**<span class="hljs-attribute">var</span> <span class="hljs-title">resource_tree</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-current_resource_list" href="#property-current_resource_list">**<span class="hljs-attribute">var</span> <span class="hljs-title">current_resource_list</span> <span style = "color: gray"> = </span> []** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-sort_mode" href="#property-sort_mode">**<span class="hljs-attribute">var</span> <span class="hljs-title">sort_mode</span> <span style = "color: gray"> = </span> 0** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-clean_resource_list" href="#method-clean_resource_list">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clean_resource_list</span>](#method-clean_resource_list) ( `resources_list`: [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) = `[]` )</a>  ⇒ <span class="hljs-attribute">[PackedStringArray](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_resource_list" href="#method-update_resource_list">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_resource_list</span>](#method-update_resource_list) ( `resources_list`: [PackedStringArray](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray) = `[]` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-add_item" href="#method-add_item">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_item</span>](#method-add_item) ( `item`: [DialogicSidebar.ResourceListItem](class_dialogicsidebar.resourcelistitem.md), `parent`: [TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem), `current_file`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-add_folder_item" href="#method-add_folder_item">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_folder_item</span>](#method-add_folder_item) ( `label`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `parent`: [TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem) )</a>  ⇒ <span class="hljs-attribute">[TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_unsaved_indicator" href="#method-set_unsaved_indicator">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_unsaved_indicator</span>](#method-set_unsaved_indicator) ( `saved`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_content_list" href="#method-update_content_list">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_content_list</span>](#method-update_content_list) ( `list`: [PackedStringArray](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-remove_item_from_list" href="#method-remove_item_from_list">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_item_from_list</span>](#method-remove_item_from_list) ( `item`: [TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-edit_resource" href="#method-edit_resource">**<span class="hljs-attribute">func</span> [<span class="hljs-title">edit_resource</span>](#method-edit_resource) ( `resource_item`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

