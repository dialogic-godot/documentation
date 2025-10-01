
<div class="header-banner purple">
<div class="header-label purple">DialogicUtil</div>
</div>

*This contains the source code documentation of the class `DialogicUtil`.*
        
# DialogicUtil
**Inherits:** [RefCounted](https://docs.godotengine.org/en/latest/classes/class_refcounted.html#class-refcounted)

Script that container helper methods for both editor and game execution. Used whenever the same thing is needed in different parts of the plugin.
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span> | [<span class="hljs-title">get_editor_scale</span>](#method-get_editor_scale) ( ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">get_dialogic_plugin</span>](#method-get_dialogic_plugin) ( ) 
<span class="hljs-attribute">[DialogicGameHandler](class_dialogicgamehandler.md)</span> | [<span class="hljs-title">autoload</span>](#method-autoload) ( ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">listdir</span>](#method-listdir) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `files_only`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `_throw_error`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `full_file_path`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `include_imports`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_module_path</span>](#method-get_module_path) ( `name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `builtin`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span class="hljs-attribute">[DialogicIndexer[]](https://docs.godotengine.org/en/latest/classes/class_dialogicindexer.html#class-dialogicindexer)</span> | [<span class="hljs-title">get_indexers</span>](#method-get_indexers) ( `include_custom`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `force_reload`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">pretty_name</span>](#method-pretty_name) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_editor_setting</span>](#method-set_editor_setting) ( `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">get_editor_setting</span>](#method-get_editor_setting) ( `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null` ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_color_palette</span>](#method-get_color_palette) ( `default`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">[Color](https://docs.godotengine.org/en/latest/classes/class_color.html#class-color)</span> | [<span class="hljs-title">get_color</span>](#method-get_color) ( `value`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_physics_timer</span>](#method-is_physics_timer) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_timer_process_callback</span>](#method-update_timer_process_callback) ( `timer`: [Timer](https://docs.godotengine.org/en/latest/classes/class_timer.html#class-timer) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">multitween</span>](#method-multitween) ( `tweened_value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `item`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node), `property`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `part`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_next_translation_id</span>](#method-get_next_translation_id) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_default_variables</span>](#method-get_default_variables) ( ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">list_variables</span>](#method-list_variables) ( `dict`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">get_variable_value_type</span>](#method-get_variable_value_type) ( `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">get_variable_type</span>](#method-get_variable_type) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `dict`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">apply_scene_export_overrides</span>](#method-apply_scene_export_overrides) ( `node`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node), `export_overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `apply`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_scene_export_defaults</span>](#method-get_scene_export_defaults) ( `node`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">make_file_custom</span>](#method-make_file_custom) ( `original_file`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `target_folder`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_file_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `new_folder_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">customize_file</span>](#method-customize_file) ( `original_file`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `target_file`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)</span> | [<span class="hljs-title">setup_script_property_edit_node</span>](#method-setup_script_property_edit_node) ( `property_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `property_changed`: [Callable](https://docs.godotengine.org/en/latest/classes/class_callable.html#class-callable) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_custom_event_defaults</span>](#method-get_custom_event_defaults) ( `event_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">str_to_bool</span>](#method-str_to_bool) ( `boolstring`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">logical_convert</span>](#method-logical_convert) ( `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">str_to_hash_set</span>](#method-str_to_hash_set) ( `source`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_character_suggestions</span>](#method-get_character_suggestions) ( `_search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `current_value`: [DialogicCharacter](class_dialogiccharacter.md) = `null`, `allow_none`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `allow_all`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `editor_node`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) = `null` ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_portrait_suggestions</span>](#method-get_portrait_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `character`: [DialogicCharacter](class_dialogiccharacter.md), `allow_empty`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `empty_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `"Don\'t Change"` ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_portrait_position_suggestions</span>](#method-get_portrait_position_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_autoload_suggestions</span>](#method-get_autoload_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[Script](https://docs.godotengine.org/en/latest/classes/class_script.html#class-script)</span> | [<span class="hljs-title">get_autoload_script_resource</span>](#method-get_autoload_script_resource) ( `autoload_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_autoload_method_suggestions</span>](#method-get_autoload_method_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `autoload_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_autoload_property_suggestions</span>](#method-get_autoload_property_suggestions) ( `_filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `autoload_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_audio_bus_suggestions</span>](#method-get_audio_bus_suggestions) ( `_filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_audio_channel_suggestions</span>](#method-get_audio_channel_suggestions) ( `_search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_audio_channel_defaults</span>](#method-get_audio_channel_defaults) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">validate_audio_channel_name</span>](#method-validate_audio_channel_name) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
--- 
## Constants


<a class="header" id="constant-ANY" href="#constant-ANY">**<span class="hljs-attribute">const</span> <span class="hljs-title">ANY</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-STRING" href="#constant-STRING">**<span class="hljs-attribute">const</span> <span class="hljs-title">STRING</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-FLOAT" href="#constant-FLOAT">**<span class="hljs-attribute">const</span> <span class="hljs-title">FLOAT</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-INT" href="#constant-INT">**<span class="hljs-attribute">const</span> <span class="hljs-title">INT</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-BOOL" href="#constant-BOOL">**<span class="hljs-attribute">const</span> <span class="hljs-title">BOOL</span><span class="hljs-comment"> = 4</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Method Descriptions



<a class="header" id="method-get_editor_scale" href="#method-get_editor_scale">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_editor_scale</span>](#method-get_editor_scale) ( )</a>  ⇒ <span class="hljs-attribute">[float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)</span>** 



This method should be used instead of EditorInterface.get_editor_scale(), because if you use that it will run perfectly fine from the editor, but crash when the game is exported.

---



<a class="header" id="method-get_dialogic_plugin" href="#method-get_dialogic_plugin">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_dialogic_plugin</span>](#method-get_dialogic_plugin) ( )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



Although this does in fact always return a EditorPlugin node, that class is apparently not present in export and referencing it here creates a crash.

---



<a class="header" id="method-autoload" href="#method-autoload">**<span class="hljs-attribute">func</span> [<span class="hljs-title">autoload</span>](#method-autoload) ( )</a>  ⇒ <span class="hljs-attribute">[DialogicGameHandler](class_dialogicgamehandler.md)</span>** 



Returns the autoload when in-game.

---



<a class="header" id="method-listdir" href="#method-listdir">**<span class="hljs-attribute">func</span> [<span class="hljs-title">listdir</span>](#method-listdir) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `files_only`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `_throw_error`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `full_file_path`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `include_imports`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



##############################################################################

---



<a class="header" id="method-get_module_path" href="#method-get_module_path">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_module_path</span>](#method-get_module_path) ( `name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `builtin`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_indexers" href="#method-get_indexers">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_indexers</span>](#method-get_indexers) ( `include_custom`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `force_reload`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[DialogicIndexer[]](https://docs.godotengine.org/en/latest/classes/class_dialogicindexer.html#class-dialogicindexer)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-pretty_name" href="#method-pretty_name">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pretty_name</span>](#method-pretty_name) ( `file_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Turns a `file_path` from `some_file.png` to `Some File`.

---



<a class="header" id="method-set_editor_setting" href="#method-set_editor_setting">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_editor_setting</span>](#method-set_editor_setting) ( `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_editor_setting" href="#method-get_editor_setting">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_editor_setting</span>](#method-get_editor_setting) ( `setting`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null` )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_color_palette" href="#method-get_color_palette">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_color_palette</span>](#method-get_color_palette) ( `default`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_color" href="#method-get_color">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_color</span>](#method-get_color) ( `value`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Color](https://docs.godotengine.org/en/latest/classes/class_color.html#class-color)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_physics_timer" href="#method-is_physics_timer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_physics_timer</span>](#method-is_physics_timer) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



##############################################################################

---



<a class="header" id="method-update_timer_process_callback" href="#method-update_timer_process_callback">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_timer_process_callback</span>](#method-update_timer_process_callback) ( `timer`: [Timer](https://docs.godotengine.org/en/latest/classes/class_timer.html#class-timer) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-multitween" href="#method-multitween">**<span class="hljs-attribute">func</span> [<span class="hljs-title">multitween</span>](#method-multitween) ( `tweened_value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `item`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node), `property`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `part`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



##############################################################################

---



<a class="header" id="method-get_next_translation_id" href="#method-get_next_translation_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_next_translation_id</span>](#method-get_next_translation_id) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_default_variables" href="#method-get_default_variables">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_default_variables</span>](#method-get_default_variables) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-list_variables" href="#method-list_variables">**<span class="hljs-attribute">func</span> [<span class="hljs-title">list_variables</span>](#method-list_variables) ( `dict`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_variable_value_type" href="#method-get_variable_value_type">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_variable_value_type</span>](#method-get_variable_value_type) ( `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_variable_type" href="#method-get_variable_type">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_variable_type</span>](#method-get_variable_type) ( `path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `dict`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `{}` )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-apply_scene_export_overrides" href="#method-apply_scene_export_overrides">**<span class="hljs-attribute">func</span> [<span class="hljs-title">apply_scene_export_overrides</span>](#method-apply_scene_export_overrides) ( `node`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node), `export_overrides`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `apply`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_scene_export_defaults" href="#method-get_scene_export_defaults">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_scene_export_defaults</span>](#method-get_scene_export_defaults) ( `node`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-make_file_custom" href="#method-make_file_custom">**<span class="hljs-attribute">func</span> [<span class="hljs-title">make_file_custom</span>](#method-make_file_custom) ( `original_file`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `target_folder`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `new_file_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `new_folder_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-customize_file" href="#method-customize_file">**<span class="hljs-attribute">func</span> [<span class="hljs-title">customize_file</span>](#method-customize_file) ( `original_file`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `target_file`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-setup_script_property_edit_node" href="#method-setup_script_property_edit_node">**<span class="hljs-attribute">func</span> [<span class="hljs-title">setup_script_property_edit_node</span>](#method-setup_script_property_edit_node) ( `property_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `property_changed`: [Callable](https://docs.godotengine.org/en/latest/classes/class_callable.html#class-callable) )</a>  ⇒ <span class="hljs-attribute">[Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_custom_event_defaults" href="#method-get_custom_event_defaults">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_custom_event_defaults</span>](#method-get_custom_event_defaults) ( `event_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-str_to_bool" href="#method-str_to_bool">**<span class="hljs-attribute">func</span> [<span class="hljs-title">str_to_bool</span>](#method-str_to_bool) ( `boolstring`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-logical_convert" href="#method-logical_convert">**<span class="hljs-attribute">func</span> [<span class="hljs-title">logical_convert</span>](#method-logical_convert) ( `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-str_to_hash_set" href="#method-str_to_hash_set">**<span class="hljs-attribute">func</span> [<span class="hljs-title">str_to_hash_set</span>](#method-str_to_hash_set) ( `source`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Takes `source` and builds a dictionary of keys only. The values are `null`.

---



<a class="header" id="method-get_character_suggestions" href="#method-get_character_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_suggestions</span>](#method-get_character_suggestions) ( `_search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `current_value`: [DialogicCharacter](class_dialogiccharacter.md) = `null`, `allow_none`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `allow_all`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `editor_node`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) = `null` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_portrait_suggestions" href="#method-get_portrait_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_portrait_suggestions</span>](#method-get_portrait_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `character`: [DialogicCharacter](class_dialogiccharacter.md), `allow_empty`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `empty_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `"Don\'t Change"` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_portrait_position_suggestions" href="#method-get_portrait_position_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_portrait_position_suggestions</span>](#method-get_portrait_position_suggestions) ( `search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_autoload_suggestions" href="#method-get_autoload_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_autoload_suggestions</span>](#method-get_autoload_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_autoload_script_resource" href="#method-get_autoload_script_resource">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_autoload_script_resource</span>](#method-get_autoload_script_resource) ( `autoload_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Script](https://docs.godotengine.org/en/latest/classes/class_script.html#class-script)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_autoload_method_suggestions" href="#method-get_autoload_method_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_autoload_method_suggestions</span>](#method-get_autoload_method_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `autoload_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_autoload_property_suggestions" href="#method-get_autoload_property_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_autoload_property_suggestions</span>](#method-get_autoload_property_suggestions) ( `_filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `autoload_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_audio_bus_suggestions" href="#method-get_audio_bus_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_audio_bus_suggestions</span>](#method-get_audio_bus_suggestions) ( `_filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_audio_channel_suggestions" href="#method-get_audio_channel_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_audio_channel_suggestions</span>](#method-get_audio_channel_suggestions) ( `_search_text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_audio_channel_defaults" href="#method-get_audio_channel_defaults">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_audio_channel_defaults</span>](#method-get_audio_channel_defaults) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-validate_audio_channel_name" href="#method-validate_audio_channel_name">**<span class="hljs-attribute">func</span> [<span class="hljs-title">validate_audio_channel_name</span>](#method-validate_audio_channel_name) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

