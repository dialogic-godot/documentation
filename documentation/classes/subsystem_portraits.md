
<div class="header-banner purple">
<div class="header-label purple">Portraits</div>
</div>

*This contains the source code documentation of the class `subsystem_Portraits`.*
        
# subsystem_Portraits
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that manages portraits and portrait positions.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">default_portrait_scene</span>](#property-default_portrait_scene) | [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene) |  `load(...)` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `_load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">pause</span>](#method-pause) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume</span>](#method-resume) ( ) 
<span class="hljs-attribute">[DialogicPortrait](class_dialogicportrait.md)</span> | [<span class="hljs-title">get_character_portrait</span>](#method-get_character_portrait) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">z_sort_portrait_containers</span>](#method-z_sort_portrait_containers) ( `con1`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `con2`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_valid_portrait</span>](#method-get_valid_portrait) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">join_character</span>](#method-join_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `mirrored`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `z_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0`, `extra_data`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">add_character</span>](#method-add_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_character_portrait</span>](#method-change_character_portrait) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `fade_animation`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `fade_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `-1.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_character_mirror</span>](#method-change_character_mirror) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `mirrored`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `force`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_character_z_index</span>](#method-change_character_z_index) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `z_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `update_zindex`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_character_extradata</span>](#method-change_character_extradata) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `extra_data`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[DialogicAnimation](class_dialogicanimation.md)</span> | [<span class="hljs-title">animate_character</span>](#method-animate_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `animation_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float), `repeats`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `1`, `is_reversed`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">move_character</span>](#method-move_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `easing`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `2`, `trans`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `1` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">leave_character</span>](#method-leave_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">leave_all_characters</span>](#method-leave_all_characters) ( `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">get_character_node</span>](#method-get_character_node) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">remove_character</span>](#method-remove_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_character_joined</span>](#method-is_character_joined) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) ) 
<span class="hljs-attribute">[DialogicCharacter[]](https://docs.godotengine.org/en/latest/classes/class_dialogiccharacter.html#class-dialogiccharacter)</span> | [<span class="hljs-title">get_joined_characters</span>](#method-get_joined_characters) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_character_info</span>](#method-get_character_info) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_speaker</span>](#method-change_speaker) ( `speaker`: [DialogicCharacter](class_dialogiccharacter.md) = `null`, `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">text_effect_portrait</span>](#method-text_effect_portrait) ( `_text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `_skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">text_effect_extradata</span>](#method-text_effect_extradata) ( `_text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `_skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
--- 

## Signals


<a class="header" id="signal-character_joined" href="#signal-character_joined">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">character_joined</span>](#signal-character_joined) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-character_left" href="#signal-character_left">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">character_left</span>](#signal-character_left) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-character_portrait_changed" href="#signal-character_portrait_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">character_portrait_changed</span>](#signal-character_portrait_changed) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-character_moved" href="#signal-character_moved">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">character_moved</span>](#signal-character_moved) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-default_portrait_scene" href="#property-default_portrait_scene">**<span class="hljs-attribute">var</span> <span class="hljs-title">default_portrait_scene</span> <span style = "color: gray"> = </span> load(...)** 



The default portrait scene.

---

## Method Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-load_game_state" href="#method-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#method-load_game_state) ( `_load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-pause" href="#method-pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pause</span>](#method-pause) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-resume" href="#method-resume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume</span>](#method-resume) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_character_portrait" href="#method-get_character_portrait">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_portrait</span>](#method-get_character_portrait) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) )</a>  ⇒ <span class="hljs-attribute">[DialogicPortrait](class_dialogicportrait.md)</span>** 



Checks if [para, character] has joined the scene, if so, returns its active  node.  The difference between an active and inactive nodes is whether the node is the latest node. 
If a portrait is fading/animating from portrait A and B, both will exist in the scene, but only the new portrait is active, even if it is not fully visible yet.

---



<a class="header" id="method-z_sort_portrait_containers" href="#method-z_sort_portrait_containers">**<span class="hljs-attribute">func</span> [<span class="hljs-title">z_sort_portrait_containers</span>](#method-z_sort_portrait_containers) ( `con1`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `con2`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_valid_portrait" href="#method-get_valid_portrait">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_valid_portrait</span>](#method-get_valid_portrait) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Checks multiple cases to return a valid portrait to use.

---



<a class="header" id="method-join_character" href="#method-join_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">join_character</span>](#method-join_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `mirrored`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `z_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0`, `extra_data`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



Adds a character at a position and sets it's portrait. If the character is already joined it will only update, portrait, position, etc.

---



<a class="header" id="method-add_character" href="#method-add_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_character</span>](#method-add_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `container`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-change_character_portrait" href="#method-change_character_portrait">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_character_portrait</span>](#method-change_character_portrait) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `fade_animation`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `fade_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `-1.0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Changes the portrait of a character. Only works with joined characters.

---



<a class="header" id="method-change_character_mirror" href="#method-change_character_mirror">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_character_mirror</span>](#method-change_character_mirror) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `mirrored`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `force`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



Changes the mirror of the given character. Only works with joined characters

---



<a class="header" id="method-change_character_z_index" href="#method-change_character_z_index">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_character_z_index</span>](#method-change_character_z_index) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `z_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `update_zindex`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span style = "color: gray">void</span>** 



Changes the z_index of a character. Only works with joined characters

---



<a class="header" id="method-change_character_extradata" href="#method-change_character_extradata">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_character_extradata</span>](#method-change_character_extradata) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `extra_data`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



Changes the extra data on the given character. Only works with joined characters

---



<a class="header" id="method-animate_character" href="#method-animate_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">animate_character</span>](#method-animate_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `animation_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float), `repeats`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `1`, `is_reversed`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[DialogicAnimation](class_dialogicanimation.md)</span>** 



Starts the given animation on the given character. Only works with joined characters

---



<a class="header" id="method-move_character" href="#method-move_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">move_character</span>](#method-move_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `position_id`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `easing`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `2`, `trans`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `1` )</a>  ⇒ <span style = "color: gray">void</span>** 



Moves the given character to the given position. Only works with joined characters

---



<a class="header" id="method-leave_character" href="#method-leave_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">leave_character</span>](#method-leave_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



Removes a character with a given animation or the default animation.

---



<a class="header" id="method-leave_all_characters" href="#method-leave_all_characters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">leave_all_characters</span>](#method-leave_all_characters) ( `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



Removes all joined characters with a given animation or the default animation.

---



<a class="header" id="method-get_character_node" href="#method-get_character_node">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_node</span>](#method-get_character_node) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



Finds the character node for a `character`. Return `null` if the `character` is not part of the scene.

---



<a class="header" id="method-remove_character" href="#method-remove_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_character</span>](#method-remove_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Removes the given characters portrait. Only works with joined characters.

---



<a class="header" id="method-is_character_joined" href="#method-is_character_joined">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_character_joined</span>](#method-is_character_joined) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns true if the given character is currently joined.

---



<a class="header" id="method-get_joined_characters" href="#method-get_joined_characters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_joined_characters</span>](#method-get_joined_characters) ( )</a>  ⇒ <span class="hljs-attribute">[DialogicCharacter[]](https://docs.godotengine.org/en/latest/classes/class_dialogiccharacter.html#class-dialogiccharacter)</span>** 



Returns a list of the joined charcters (as resources)

---



<a class="header" id="method-get_character_info" href="#method-get_character_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_info</span>](#method-get_character_info) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Returns a dictionary with info on a given character. Keys can be [joined, character, node (for the portrait node), position_id] Only joined is included (and false) for not joined characters

---



<a class="header" id="method-change_speaker" href="#method-change_speaker">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_speaker</span>](#method-change_speaker) ( `speaker`: [DialogicCharacter](class_dialogiccharacter.md) = `null`, `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



Updates all portrait containers set to SPEAKER.

---



<a class="header" id="method-text_effect_portrait" href="#method-text_effect_portrait">**<span class="hljs-attribute">func</span> [<span class="hljs-title">text_effect_portrait</span>](#method-text_effect_portrait) ( `_text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `_skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Called from the [portrait=something] text effect.

---



<a class="header" id="method-text_effect_extradata" href="#method-text_effect_extradata">**<span class="hljs-attribute">func</span> [<span class="hljs-title">text_effect_extradata</span>](#method-text_effect_extradata) ( `_text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `_skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Called from the [extra_data=something] text effect.

---

