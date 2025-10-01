
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
[<span class="hljs-title">name</span>](#property-name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"Style"` 
[<span class="hljs-title">inherits</span>](#property-inherits) | [DialogicStyle](class_dialogicstyle.md) |  `null` 
[<span class="hljs-title">layer_list</span>](#property-layer_list) | [String[]](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `[]` 
[<span class="hljs-title">layer_info</span>](#property-layer_info) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{...}` 
[<span class="hljs-title">base_scene</span>](#property-base_scene) | [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene) |  `null` 
[<span class="hljs-title">base_overrides</span>](#property-base_overrides) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{}` 
[<span class="hljs-title">layers</span>](#property-layers) | [DialogicStyleLayer[]](https://docs.godotengine.org/en/latest/classes/class_dialogicstylelayer.html#class-dialogicstylelayer) |  `[]` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">get_layer_count</span>](#method-get_layer_count) ( ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">get_layer_index</span>](#method-get_layer_index) ( `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_layer</span>](#method-has_layer) ( `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_layer_index</span>](#method-has_layer_index) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_layer_id_at_index</span>](#method-get_layer_id_at_index) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_layer_info</span>](#method-get_layer_info) ( `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_new_layer_id</span>](#method-get_new_layer_id) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">add_layer</span>](#method-add_layer) ( `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}`, `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `"##"` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">delete_layer</span>](#method-delete_layer) ( `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">move_layer</span>](#method-move_layer) ( `from_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `to_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_layer_scene</span>](#method-set_layer_scene) ( `layer_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_layer_overrides</span>](#method-set_layer_overrides) ( `layer_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_layer_setting</span>](#method-set_layer_setting) ( `layer_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">remove_layer_setting</span>](#method-remove_layer_setting) ( `layer_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">inherits_anything</span>](#method-inherits_anything) ( ) 
<span class="hljs-attribute">[DialogicStyle](class_dialogicstyle.md)</span> | [<span class="hljs-title">get_inheritance_root</span>](#method-get_inheritance_root) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">merge_layer_infos</span>](#method-merge_layer_infos) ( `new_layer_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `ancestor_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_layer_inherited_info</span>](#method-get_layer_inherited_info) ( `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `inherited_only`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_layer_inherited_list</span>](#method-get_layer_inherited_list) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">realize_inheritance</span>](#method-realize_inheritance) ( ) 
<span class="hljs-attribute">[DialogicStyle](class_dialogicstyle.md)</span> | [<span class="hljs-title">clone</span>](#method-clone) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">prepare</span>](#method-prepare) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_from_pre_alpha16</span>](#method-update_from_pre_alpha16) ( ) 
--- 
## Property Descriptions



<a class="header" id="property-name" href="#property-name">**<span class="hljs-attribute">var</span> <span class="hljs-title">name</span> <span style = "color: gray"> = </span> "Style"** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-inherits" href="#property-inherits">**<span class="hljs-attribute">var</span> <span class="hljs-title">inherits</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-layer_list" href="#property-layer_list">**<span class="hljs-attribute">var</span> <span class="hljs-title">layer_list</span> <span style = "color: gray"> = </span> []** 



Stores the layer order

---



<a class="header" id="property-layer_info" href="#property-layer_info">**<span class="hljs-attribute">var</span> <span class="hljs-title">layer_info</span> <span style = "color: gray"> = </span> {...}** 



Stores the layer infos

---



<a class="header" id="property-base_scene" href="#property-base_scene">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_scene</span> <span style = "color: gray"> = </span> null** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-base_overrides" href="#property-base_overrides">**<span class="hljs-attribute">var</span> <span class="hljs-title">base_overrides</span> <span style = "color: gray"> = </span> {}** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-layers" href="#property-layers">**<span class="hljs-attribute">var</span> <span class="hljs-title">layers</span> <span style = "color: gray"> = </span> []** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-get_layer_count" href="#method-get_layer_count">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer_count</span>](#method-get_layer_count) ( )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



Returns the amount of layers (the base layer is not included).

---



<a class="header" id="method-get_layer_index" href="#method-get_layer_index">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer_index</span>](#method-get_layer_index) ( `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



Returns the index of the layer with `id` in the layer list. Returns -1 for the base layer (id=="") which is not in the layer list.

---



<a class="header" id="method-has_layer" href="#method-has_layer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_layer</span>](#method-has_layer) ( `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns `true` if `id` is a valid id for a layer.

---



<a class="header" id="method-has_layer_index" href="#method-has_layer_index">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_layer_index</span>](#method-has_layer_index) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns `true` if `index` is a valid index for a layer.

---



<a class="header" id="method-get_layer_id_at_index" href="#method-get_layer_id_at_index">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer_id_at_index</span>](#method-get_layer_id_at_index) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the id of the layer at `index`.

---



<a class="header" id="method-get_layer_info" href="#method-get_layer_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer_info</span>](#method-get_layer_info) ( `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_new_layer_id" href="#method-get_new_layer_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_new_layer_id</span>](#method-get_new_layer_id) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns a new layer id not yet in use.

---



<a class="header" id="method-add_layer" href="#method-add_layer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_layer</span>](#method-add_layer) ( `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}`, `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `"##"` )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Adds a layer with the given scene and overrides. Returns the new layers id.

---



<a class="header" id="method-delete_layer" href="#method-delete_layer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">delete_layer</span>](#method-delete_layer) ( `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Deletes the layer with the given id. Deleting the base layer is not allowed.

---



<a class="header" id="method-move_layer" href="#method-move_layer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">move_layer</span>](#method-move_layer) ( `from_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `to_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span style = "color: gray">void</span>** 



Moves the layer at `from_index` to `to_index`.

---



<a class="header" id="method-set_layer_scene" href="#method-set_layer_scene">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_layer_scene</span>](#method-set_layer_scene) ( `layer_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Changes the scene property of the DialogicStyleLayer resource at `layer_id`.

---



<a class="header" id="method-set_layer_overrides" href="#method-set_layer_overrides">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_layer_overrides</span>](#method-set_layer_overrides) ( `layer_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_layer_setting" href="#method-set_layer_setting">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_layer_setting</span>](#method-set_layer_setting) ( `layer_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span style = "color: gray">void</span>** 



Changes an override of the DialogicStyleLayer resource at `layer_id`.

---



<a class="header" id="method-remove_layer_setting" href="#method-remove_layer_setting">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_layer_setting</span>](#method-remove_layer_setting) ( `layer_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Resets (removes) an override of the DialogicStyleLayer resource at `layer_id`.

---



<a class="header" id="method-inherits_anything" href="#method-inherits_anything">**<span class="hljs-attribute">func</span> [<span class="hljs-title">inherits_anything</span>](#method-inherits_anything) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns `true` if this style is inheriting from another style.

---



<a class="header" id="method-get_inheritance_root" href="#method-get_inheritance_root">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_inheritance_root</span>](#method-get_inheritance_root) ( )</a>  ⇒ <span class="hljs-attribute">[DialogicStyle](class_dialogicstyle.md)</span>** 



Returns the base style of this style.

---



<a class="header" id="method-merge_layer_infos" href="#method-merge_layer_infos">**<span class="hljs-attribute">func</span> [<span class="hljs-title">merge_layer_infos</span>](#method-merge_layer_infos) ( `new_layer_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `ancestor_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



This merges some `layer_info` with it's param ancestors layer info.

---



<a class="header" id="method-get_layer_inherited_info" href="#method-get_layer_inherited_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer_inherited_info</span>](#method-get_layer_inherited_info) ( `id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `inherited_only`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Returns the layer info of the layer at `id` taking into account inherited info. If `inherited_only` is `true`, the local info is not included.

---



<a class="header" id="method-get_layer_inherited_list" href="#method-get_layer_inherited_list">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer_inherited_list</span>](#method-get_layer_inherited_list) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



Returns the layer list of the root style.

---



<a class="header" id="method-realize_inheritance" href="#method-realize_inheritance">**<span class="hljs-attribute">func</span> [<span class="hljs-title">realize_inheritance</span>](#method-realize_inheritance) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Applies inherited info to the local layers. Then removes inheritance.

---



<a class="header" id="method-clone" href="#method-clone">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clone</span>](#method-clone) ( )</a>  ⇒ <span class="hljs-attribute">[DialogicStyle](class_dialogicstyle.md)</span>** 



Creates a fresh new style with the same settings.

---



<a class="header" id="method-prepare" href="#method-prepare">**<span class="hljs-attribute">func</span> [<span class="hljs-title">prepare</span>](#method-prepare) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Starts preloading all the scenes used by this style.

---



<a class="header" id="method-update_from_pre_alpha16" href="#method-update_from_pre_alpha16">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_from_pre_alpha16</span>](#method-update_from_pre_alpha16) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

