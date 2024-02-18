
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
character_editor | [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control) |   
hint_text | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
selected_item | [TreeItem](https://docs.godotengine.org/en/latest/classes/class_treeitem.html#class-treeitem) |  `null` 

## Signals


<a class="header" id="signal-changed" href="#signal-changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">changed</span>](#signal-changed) ( )** </a>



Emit this, if something changed

---



<a class="header" id="signal-update_preview" href="#signal-update_preview">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">update_preview</span>](#signal-update_preview) ( )** </a>



Emit this if the preview should reload

---

