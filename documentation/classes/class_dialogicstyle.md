
<div class="header-banner purple">
<div class="header-label purple">DialogicStyle</div>
</div>

*This contains the source code documentation of the class `DialogicStyle`.*
        
# DialogicStyle
**Inherits:** Resource

A style represents a collection of layers and settings. A style can inherit from another style.
## Properties
Name | Type | Default 
--- | --- | --- 
base_overrides | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
base_scene | [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene) |  `null` 
inherits | [DialogicStyle](class_dialogicstyle.md) |  `null` 
layers | [DialogicStyleLayer[]](https://docs.godotengine.org/en/latest/classes/class_dialogicstylelayer.html#class-dialogicstylelayer) |   
name | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"Style"` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_layer</span>](#property-add_layer) ( `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">clone</span>](#property-clone) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">delete_layer</span>](#property-delete_layer) ( `layer_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_base_scene</span>](#property-get_base_scene) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_inheritance_root</span>](#property-get_inheritance_root) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_layer_count</span>](#property-get_layer_count) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_layer_info</span>](#property-get_layer_info) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_layer_inherited_info</span>](#property-get_layer_inherited_info) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `inherited_only`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_layer_list</span>](#property-get_layer_list) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">has_layer</span>](#property-has_layer) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">inherits_anything</span>](#property-inherits_anything) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">merge_layer_infos</span>](#property-merge_layer_infos) ( `layer_a`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `layer_b`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">move_layer</span>](#property-move_layer) ( `from_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `to_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">prepare</span>](#property-prepare) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">realize_inheritance</span>](#property-realize_inheritance) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">remove_layer_setting</span>](#property-remove_layer_setting) ( `layer`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">set_layer_scene</span>](#property-set_layer_scene) ( `layer_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">set_layer_setting</span>](#property-set_layer_setting) ( `layer`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
--- 
## Property Descriptions



<a class="header" id="property-add_layer" href="#property-add_layer">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_layer</span>](#property-add_layer) ( `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-clone" href="#property-clone">**<span class="hljs-attribute">void</span> [<span class="hljs-title">clone</span>](#property-clone) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-delete_layer" href="#property-delete_layer">**<span class="hljs-attribute">void</span> [<span class="hljs-title">delete_layer</span>](#property-delete_layer) ( `layer_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_base_scene" href="#property-get_base_scene">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_base_scene</span>](#property-get_base_scene) ( )** </a>



This always returns the inheritance root's scene!

---



<a class="header" id="property-get_inheritance_root" href="#property-get_inheritance_root">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_inheritance_root</span>](#property-get_inheritance_root) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_layer_count" href="#property-get_layer_count">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_layer_count</span>](#property-get_layer_count) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_layer_info" href="#property-get_layer_info">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_layer_info</span>](#property-get_layer_info) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_layer_inherited_info" href="#property-get_layer_inherited_info">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_layer_inherited_info</span>](#property-get_layer_inherited_info) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `inherited_only`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_layer_list" href="#property-get_layer_list">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_layer_list</span>](#property-get_layer_list) ( )** </a>



This always returns the full inherited roots layers!

---



<a class="header" id="property-has_layer" href="#property-has_layer">**<span class="hljs-attribute">void</span> [<span class="hljs-title">has_layer</span>](#property-has_layer) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-inherits_anything" href="#property-inherits_anything">**<span class="hljs-attribute">void</span> [<span class="hljs-title">inherits_anything</span>](#property-inherits_anything) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-merge_layer_infos" href="#property-merge_layer_infos">**<span class="hljs-attribute">void</span> [<span class="hljs-title">merge_layer_infos</span>](#property-merge_layer_infos) ( `layer_a`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `layer_b`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



This merges two layers (mainly their overrides). Layer a has priority!

---



<a class="header" id="property-move_layer" href="#property-move_layer">**<span class="hljs-attribute">void</span> [<span class="hljs-title">move_layer</span>](#property-move_layer) ( `from_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `to_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-prepare" href="#property-prepare">**<span class="hljs-attribute">void</span> [<span class="hljs-title">prepare</span>](#property-prepare) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-realize_inheritance" href="#property-realize_inheritance">**<span class="hljs-attribute">void</span> [<span class="hljs-title">realize_inheritance</span>](#property-realize_inheritance) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-remove_layer_setting" href="#property-remove_layer_setting">**<span class="hljs-attribute">void</span> [<span class="hljs-title">remove_layer_setting</span>](#property-remove_layer_setting) ( `layer`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_layer_scene" href="#property-set_layer_scene">**<span class="hljs-attribute">void</span> [<span class="hljs-title">set_layer_scene</span>](#property-set_layer_scene) ( `layer_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_layer_setting" href="#property-set_layer_setting">**<span class="hljs-attribute">void</span> [<span class="hljs-title">set_layer_setting</span>](#property-set_layer_setting) ( `layer`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

