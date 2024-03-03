
<div class="header-banner purple">
<div class="header-label purple">subsystem_Styles</div>
</div>

*This contains the source code documentation of the class `subsystem_Styles`.*
        
# subsystem_Styles
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

##################################################################################################
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[DialogicLayoutBase](class_dialogiclayoutbase.md)</span> | [<span class="hljs-title">create_layout</span>](#method-create_layout) ( `style`: [DialogicStyle](class_dialogicstyle.md), `parent`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) = `null` ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_current_style</span>](#method-get_current_style) ( ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">get_first_node_in_layout</span>](#method-get_first_node_in_layout) ( `group_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">get_layout_node</span>](#method-get_layout_node) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_active_layout_node</span>](#method-has_active_layout_node) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">load_style</span>](#method-load_style) ( `style_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `parent`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) = `null`, `is_base_style`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reload_current_info_into_new_style</span>](#method-reload_current_info_into_new_style) ( ) 
--- 

## Signals


<a class="header" id="signal-style_changed" href="#signal-style_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">style_changed</span>](#signal-style_changed) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-create_layout" href="#method-create_layout">**<span class="hljs-attribute">func</span> [<span class="hljs-title">create_layout</span>](#method-create_layout) ( `style`: [DialogicStyle](class_dialogicstyle.md), `parent`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) = `null` )</a>  ⇒ <span class="hljs-attribute">[DialogicLayoutBase](class_dialogiclayoutbase.md)</span>** 



Method that adds a layout scene with all the necessary layers. The layout scene will be added to the tree root and returned.

---



<a class="header" id="method-get_current_style" href="#method-get_current_style">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_current_style</span>](#method-get_current_style) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the style currently in use

---



<a class="header" id="method-get_first_node_in_layout" href="#method-get_first_node_in_layout">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_first_node_in_layout</span>](#method-get_first_node_in_layout) ( `group_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



Similar to get_tree().get_first_node_in_group('group_name') but filtered to the active layout node subtree

---



<a class="header" id="method-get_layout_node" href="#method-get_layout_node">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layout_node</span>](#method-get_layout_node) ( )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-has_active_layout_node" href="#method-has_active_layout_node">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_active_layout_node</span>](#method-has_active_layout_node) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-load_game_state" href="#method-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-load_style" href="#method-load_style">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_style</span>](#method-load_style) ( `style_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `parent`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) = `null`, `is_base_style`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-reload_current_info_into_new_style" href="#method-reload_current_info_into_new_style">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reload_current_info_into_new_style</span>](#method-reload_current_info_into_new_style) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



When changing to a different layout scene, we have to load all the info from the current_state_info (basically

---

