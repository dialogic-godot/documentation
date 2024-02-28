
<div class="header-banner purple">
<div class="header-label purple">DialogicStyle</div>
</div>

*This contains the source code documentation of the class `DialogicStyle`.*
        
# DialogicStyle
**Inherits:** [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource)

A style represents a collection of layers and settings. A style can inherit from another style.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">base_overrides</span>](#property-base_overrides) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">base_scene</span>](#property-base_scene) | [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene) |  `null` 
[<span class="hljs-title">inherits</span>](#property-inherits) | [DialogicStyle](class_dialogicstyle.md) |  `null` 
[<span class="hljs-title">layers</span>](#property-layers) | [DialogicStyleLayer[]](https://docs.godotengine.org/en/latest/classes/class_dialogicstylelayer.html#class-dialogicstylelayer) |   
[<span class="hljs-title">name</span>](#property-name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"Style"` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_layer</span>](#property-add_layer) ( `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` ) 
<span class="hljs-attribute">[DialogicStyle](class_dialogicstyle.md)</span> | [<span class="hljs-title">clone</span>](#property-clone) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">delete_layer</span>](#property-delete_layer) ( `layer_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">[PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene)</span> | [<span class="hljs-title">get_base_scene</span>](#property-get_base_scene) ( ) 
<span class="hljs-attribute">[DialogicStyle](class_dialogicstyle.md)</span> | [<span class="hljs-title">get_inheritance_root</span>](#property-get_inheritance_root) ( ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">get_layer_count</span>](#property-get_layer_count) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_layer_info</span>](#property-get_layer_info) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_layer_inherited_info</span>](#property-get_layer_inherited_info) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `inherited_only`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">[PackedStringArray](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray)</span> | [<span class="hljs-title">get_layer_list</span>](#property-get_layer_list) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_layer</span>](#property-has_layer) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">inherits_anything</span>](#property-inherits_anything) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">merge_layer_infos</span>](#property-merge_layer_infos) ( `layer_a`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `layer_b`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">move_layer</span>](#property-move_layer) ( `from_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `to_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">prepare</span>](#property-prepare) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">realize_inheritance</span>](#property-realize_inheritance) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">remove_layer_setting</span>](#property-remove_layer_setting) ( `layer`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_layer_scene</span>](#property-set_layer_scene) ( `layer_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_layer_setting</span>](#property-set_layer_setting) ( `layer`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
--- 
## Property Descriptions



<a class="header" id="property-base_overrides" href="#property-base_overrides">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_overrides</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-base_scene" href="#property-base_scene">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_scene</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-inherits" href="#property-inherits">**<span class="hljs-attribute">var</span> <span class="hljs-title">inherits</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-layers" href="#property-layers">**<span class="hljs-attribute">var</span> <span class="hljs-title">layers</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-name" href="#property-name">**<span class="hljs-attribute">var</span> <span class="hljs-title">name</span> <span style = "color: gray"> = </span> "Style"** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-add_layer" href="#method-add_layer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_layer</span>](#property-add_layer) ( `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-clone" href="#method-clone">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clone</span>](#property-clone) ( )</a>  ⇒ <span class="hljs-attribute">[DialogicStyle](class_dialogicstyle.md)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-delete_layer" href="#method-delete_layer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">delete_layer</span>](#property-delete_layer) ( `layer_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_base_scene" href="#method-get_base_scene">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_base_scene</span>](#property-get_base_scene) ( )</a>  ⇒ <span class="hljs-attribute">[PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene)</span>** 



This always returns the inheritance root's scene!

---



<a class="header" id="method-get_inheritance_root" href="#method-get_inheritance_root">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_inheritance_root</span>](#property-get_inheritance_root) ( )</a>  ⇒ <span class="hljs-attribute">[DialogicStyle](class_dialogicstyle.md)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_layer_count" href="#method-get_layer_count">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer_count</span>](#property-get_layer_count) ( )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_layer_info" href="#method-get_layer_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer_info</span>](#property-get_layer_info) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_layer_inherited_info" href="#method-get_layer_inherited_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer_inherited_info</span>](#property-get_layer_inherited_info) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `inherited_only`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_layer_list" href="#method-get_layer_list">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer_list</span>](#property-get_layer_list) ( )</a>  ⇒ <span class="hljs-attribute">[PackedStringArray](https://docs.godotengine.org/en/latest/classes/class_packedstringarray.html#class-packedstringarray)</span>** 



This always returns the full inherited roots layers!

---



<a class="header" id="method-has_layer" href="#method-has_layer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_layer</span>](#property-has_layer) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-inherits_anything" href="#method-inherits_anything">**<span class="hljs-attribute">func</span> [<span class="hljs-title">inherits_anything</span>](#property-inherits_anything) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-merge_layer_infos" href="#method-merge_layer_infos">**<span class="hljs-attribute">func</span> [<span class="hljs-title">merge_layer_infos</span>](#property-merge_layer_infos) ( `layer_a`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `layer_b`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



This merges two layers (mainly their overrides). Layer a has priority!

---



<a class="header" id="method-move_layer" href="#method-move_layer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">move_layer</span>](#property-move_layer) ( `from_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `to_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-prepare" href="#method-prepare">**<span class="hljs-attribute">func</span> [<span class="hljs-title">prepare</span>](#property-prepare) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-realize_inheritance" href="#method-realize_inheritance">**<span class="hljs-attribute">func</span> [<span class="hljs-title">realize_inheritance</span>](#property-realize_inheritance) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-remove_layer_setting" href="#method-remove_layer_setting">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_layer_setting</span>](#property-remove_layer_setting) ( `layer`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_layer_scene" href="#method-set_layer_scene">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_layer_scene</span>](#property-set_layer_scene) ( `layer_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_layer_setting" href="#method-set_layer_setting">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_layer_setting</span>](#property-set_layer_setting) ( `layer`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

