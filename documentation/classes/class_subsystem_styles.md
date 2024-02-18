
<div class="header-banner purple">
<div class="header-label purple">subsystem_styles</div>
</div>

*This contains the source code documentation of the class `subsystem_styles`.*
        
# subsystem_styles
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

##################################################################################################
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[DialogicLayoutBase](class_dialogiclayoutbase.md)</span> | [<span class="hljs-title">create_layout</span>](#property-create_layout) ( `style`: [DialogicStyle](class_dialogicstyle.md), `parent`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) = `null` ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_current_style</span>](#property-get_current_style) ( ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">get_first_node_in_layout</span>](#property-get_first_node_in_layout) ( `group_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">get_layout_node</span>](#property-get_layout_node) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_active_layout_node</span>](#property-has_active_layout_node) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#property-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">load_style</span>](#property-load_style) ( `style_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `parent`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) = `null`, `is_base_style`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reload_current_info_into_new_style</span>](#property-reload_current_info_into_new_style) ( ) 
--- 

## Signals


<a class="header" id="signal-style_changed" href="#signal-style_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">style_changed</span>](#signal-style_changed) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-clear_game_state" href="#property-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-create_layout" href="#property-create_layout">**<span class="hljs-attribute">func</span> [<span class="hljs-title">create_layout</span>](#property-create_layout) ( `style`: [DialogicStyle](class_dialogicstyle.md), `parent`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) = `null` )</a>  ⇒ <span class="hljs-attribute">[DialogicLayoutBase](class_dialogiclayoutbase.md)</span>** 



Method that adds a layout scene with all the necessary layers. The layout scene will be added to the tree root and returned.

---



<a class="header" id="property-get_current_style" href="#property-get_current_style">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_current_style</span>](#property-get_current_style) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the style currently in use

---



<a class="header" id="property-get_first_node_in_layout" href="#property-get_first_node_in_layout">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_first_node_in_layout</span>](#property-get_first_node_in_layout) ( `group_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



Similar to get_tree().get_first_node_in_group('group_name') but filtered to the active layout node subtree

---



<a class="header" id="property-get_layout_node" href="#property-get_layout_node">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layout_node</span>](#property-get_layout_node) ( )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-has_active_layout_node" href="#property-has_active_layout_node">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_active_layout_node</span>](#property-has_active_layout_node) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-load_game_state" href="#property-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#property-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-load_style" href="#property-load_style">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_style</span>](#property-load_style) ( `style_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `parent`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) = `null`, `is_base_style`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-reload_current_info_into_new_style" href="#property-reload_current_info_into_new_style">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reload_current_info_into_new_style</span>](#property-reload_current_info_into_new_style) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



When changing to a different layout scene, we have to load all the info from the current_state_info (basically

---

