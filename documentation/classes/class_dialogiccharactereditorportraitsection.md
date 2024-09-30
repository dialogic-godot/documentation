
<div class="header-banner purple">
<div class="header-label purple">DialogicCharacterEditorPortraitSection</div>
</div>

*This contains the source code documentation of the class `DialogicCharacterEditorPortraitSection`.*
        
# DialogicCharacterEditorPortraitSection
**Inherits:** [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)

Base class for all portrait settings sections. Methods should be overriden. Changes made through fields in such a section should instantly be "saved" to the portrait_items metadata from where they will be saved to the resource.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">character_editor</span>](#property-character_editor) | [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control) |   
[<span class="hljs-title">selected_item</span>](#property-selected_item) | [TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem) |  `null` 
[<span class="hljs-title">hint_text</span>](#property-hint_text) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 

## Signals


<a class="header" id="signal-changed" href="#signal-changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">changed</span>](#signal-changed) ( )** </a>



 Emit this, if something changed 

---



<a class="header" id="signal-update_preview" href="#signal-update_preview">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">update_preview</span>](#signal-update_preview) ( )** </a>



 Emit this if the preview should reload 

---

## Property Descriptions



<a class="header" id="property-character_editor" href="#property-character_editor">**<span class="hljs-attribute">var</span> <span class="hljs-title">character_editor</span>** 



Reference to the character editor, set when instantiated

---



<a class="header" id="property-selected_item" href="#property-selected_item">**<span class="hljs-attribute">var</span> <span class="hljs-title">selected_item</span> <span style = "color: gray"> = </span> null** 



Reference to the selected portrait item. `selected_item.get_metadata(0)` can access the portraits data

---



<a class="header" id="property-hint_text" href="#property-hint_text">**<span class="hljs-attribute">var</span> <span class="hljs-title">hint_text</span> <span style = "color: gray"> = </span> ""** 



If not empty a hint icon is added to the section title

---

