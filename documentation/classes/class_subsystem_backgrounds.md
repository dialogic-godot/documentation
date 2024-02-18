
<div class="header-banner purple">
<div class="header-label purple">subsystem_backgrounds</div>
</div>

*This contains the source code documentation of the class `subsystem_backgrounds`.*
        
# subsystem_backgrounds
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

##################################################################################################
## Properties
Name | Type | Default 
--- | --- | --- 
default_background_scene | [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene) |   
default_transition | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[SubViewportContainer](https://docs.godotengine.org/en/latest/classes/class_subviewportcontainer.html#class-subviewportcontainer)</span> | [<span class="hljs-title">add_background_node</span>](#property-add_background_node) ( `scene`: [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene), `parent`: [DialogicNode_BackgroundHolder](class_dialogicnode_backgroundholder.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_background</span>](#property-has_background) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#property-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_background</span>](#property-update_background) ( `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `fade_time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `transition_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `<unknown>`, `force`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
--- 

## Signals


<a class="header" id="signal-background_changed" href="#signal-background_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">background_changed</span>](#signal-background_changed) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-add_background_node" href="#property-add_background_node">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_background_node</span>](#property-add_background_node) ( `scene`: [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene), `parent`: [DialogicNode_BackgroundHolder](class_dialogicnode_backgroundholder.md) )</a>  ⇒ <span class="hljs-attribute">[SubViewportContainer](https://docs.godotengine.org/en/latest/classes/class_subviewportcontainer.html#class-subviewportcontainer)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-clear_game_state" href="#property-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-has_background" href="#property-has_background">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_background</span>](#property-has_background) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-load_game_state" href="#property-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#property-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-update_background" href="#property-update_background">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_background</span>](#property-update_background) ( `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `fade_time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `transition_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `<unknown>`, `force`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



Method that adds a given scene as child of the DialogicNode_BackgroundHolder. It will call [_update_background()] on that scene with the given argument [argument]. It will call [_fade_in()] on that scene with the given fade time. Will call fade_out on previous backgrounds scene.  If the scene is the same as the last background you can bypass another instantiating and use the same scene. To do so implement [_should_do_background_update()] on the custom background scene. Then  [_update_background()] will be called directly on that previous scene.

---

