
<div class="header-banner purple">
<div class="header-label purple">Backgrounds</div>
</div>

*This contains the source code documentation of the class `subsystem_Backgrounds`.*
        
# subsystem_Backgrounds
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem for managing backgrounds.
## Description
This subsystem has many different helper methods for managing backgrounds. For instance, you can listen to background changes via [background_changed](#signal-background_changed).

## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">default_background_scene</span>](#property-default_background_scene) | [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene) |   
[<span class="hljs-title">default_transition</span>](#property-default_transition) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[SubViewportContainer](https://docs.godotengine.org/en/latest/classes/class_subviewportcontainer.html#class-subviewportcontainer)</span> | [<span class="hljs-title">add_background_node</span>](#method-add_background_node) ( `scene`: [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene), `parent`: [DialogicNode_BackgroundHolder](class_dialogicnode_backgroundholder.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_background</span>](#method-has_background) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `_load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_background</span>](#method-update_background) ( `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `fade_time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `transition_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `<unknown>`, `force`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
--- 

## Signals


<a class="header" id="signal-background_changed" href="#signal-background_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">background_changed</span>](#signal-background_changed) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 Whenever a new background is set, this signal is emitted and contains a dictionary with the following keys: 

Key         |   Value Type  | Value 
----------- | ------------- | ----- 
`scene`     | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) | The scene path of the new background. 
`argument`  | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) | Information given to the background on its update routine. 
`fade_time` | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float)  | The time the background may take to transition in. 
`same_scene`| [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)   | If the new background uses the same Godot scene. 
 

---

## Property Descriptions



<a class="header" id="property-default_background_scene" href="#property-default_background_scene">**<span class="hljs-attribute">var</span> <span class="hljs-title">default_background_scene</span> <span style = "color: gray"> = </span> <unknown>** 



The default background scene Dialogic will use.

---



<a class="header" id="property-default_transition" href="#property-default_transition">**<span class="hljs-attribute">var</span> <span class="hljs-title">default_transition</span> <span style = "color: gray"> = </span> <unknown>** 



The default transition Dialogic will use.

---

## Method Descriptions



<a class="header" id="method-add_background_node" href="#method-add_background_node">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_background_node</span>](#method-add_background_node) ( `scene`: [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene), `parent`: [DialogicNode_BackgroundHolder](class_dialogicnode_backgroundholder.md) )</a>  ⇒ <span class="hljs-attribute">[SubViewportContainer](https://docs.godotengine.org/en/latest/classes/class_subviewportcontainer.html#class-subviewportcontainer)</span>** 



Adds sub-viewport with the given background scene as child to Dialogic scene.

---



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Empties the current background state.

---



<a class="header" id="method-has_background" href="#method-has_background">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_background</span>](#method-has_background) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Whether a background is set.

---



<a class="header" id="method-load_game_state" href="#method-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `_load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Loads the background state from the current state info.

---



<a class="header" id="method-update_background" href="#method-update_background">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_background</span>](#method-update_background) ( `scene`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `fade_time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `transition_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `<unknown>`, `force`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



Method that adds a given scene as child of the DialogicNode_BackgroundHolder. It will call [_update_background()] on that scene with the given argument . It will call [_fade_in()] on that scene with the given fade time. Will call fade_out on previous backgrounds scene.  If the scene is the same as the last background you can bypass another instantiating and use the same scene. To do so implement [_should_do_background_update()] on the custom background scene. Then  [_update_background()] will be called directly on that previous scene.

---

