
<div class="header-banner purple">
<div class="header-label purple">subsystem_portraits</div>
</div>

*This contains the source code documentation of the class `subsystem_portraits`.*
        
# subsystem_portraits
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that manages portraits and portrait positions.
## Properties
Name | Type | Default 
--- | --- | --- 
default_portrait_scene | [PackedScene](https://docs.godotengine.org/en/latest/classes/class_packedscene.html#class-packedscene) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">add_character</span>](#property-add_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `position_idx`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_portrait_position</span>](#property-add_portrait_position) ( `position_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `position`: [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) ) 
<span class="hljs-attribute">[DialogicAnimation](class_dialogicanimation.md)</span> | [<span class="hljs-title">animate_character</span>](#property-animate_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `animation_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float), `repeats`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `1` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_character_extradata</span>](#property-change_character_extradata) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `extra_data`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_character_mirror</span>](#property-change_character_mirror) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `mirrored`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `force`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_character_portrait</span>](#property-change_character_portrait) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `update_transform`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_character_z_index</span>](#property-change_character_z_index) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `z_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `update_zindex`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">change_speaker</span>](#property-change_speaker) ( `speaker`: [DialogicCharacter](class_dialogiccharacter.md) = `null`, `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_character_info</span>](#property-get_character_info) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) ) 
<span class="hljs-attribute">[DialogicCharacter[]](https://docs.godotengine.org/en/latest/classes/class_dialogiccharacter.html#class-dialogiccharacter)</span> | [<span class="hljs-title">get_joined_characters</span>](#property-get_joined_characters) ( ) 
<span class="hljs-attribute">[DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md)</span> | [<span class="hljs-title">get_portrait_container</span>](#property-get_portrait_container) ( `postion_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_character_joined</span>](#property-is_character_joined) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">join_character</span>](#property-join_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `position_idx`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `mirrored`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `z_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0`, `extra_data`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">leave_all_characters</span>](#property-leave_all_characters) ( `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">leave_character</span>](#property-leave_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#property-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">move_character</span>](#property-move_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `position_idx`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">move_portrait_position</span>](#property-move_portrait_position) ( `position_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `vector`: [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2), `relative`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">pause</span>](#property-pause) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">remove_character</span>](#property-remove_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset_all_portrait_positions</span>](#property-reset_all_portrait_positions) ( `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset_portrait_position</span>](#property-reset_portrait_position) ( `position_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">resume</span>](#property-resume) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">text_effect_portrait</span>](#property-text_effect_portrait) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">z_sort_portrait_containers</span>](#property-z_sort_portrait_containers) ( `con1`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `con2`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md) ) 
--- 

## Signals


<a class="header" id="signal-character_joined" href="#signal-character_joined">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">character_joined</span>](#signal-character_joined) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-character_left" href="#signal-character_left">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">character_left</span>](#signal-character_left) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-character_moved" href="#signal-character_moved">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">character_moved</span>](#signal-character_moved) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-character_portrait_changed" href="#signal-character_portrait_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">character_portrait_changed</span>](#signal-character_portrait_changed) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-position_changed" href="#signal-position_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">position_changed</span>](#signal-position_changed) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-add_character" href="#property-add_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_character</span>](#property-add_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `position_idx`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-add_portrait_position" href="#property-add_portrait_position">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_portrait_position</span>](#property-add_portrait_position) ( `position_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `position`: [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) )</a>  ⇒ <span style = "color: gray">void</span>** 



Creates a new portrait container node. It will copy it's size and most settings from the first p_container in the tree. It will be added as a sibling of the first p_container in the tree.

---



<a class="header" id="property-animate_character" href="#property-animate_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">animate_character</span>](#property-animate_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `animation_path`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float), `repeats`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `1` )</a>  ⇒ <span class="hljs-attribute">[DialogicAnimation](class_dialogicanimation.md)</span>** 



Starts the given animation on the given character. Only works with joined characters

---



<a class="header" id="property-change_character_extradata" href="#property-change_character_extradata">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_character_extradata</span>](#property-change_character_extradata) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `extra_data`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



Changes the extra data on the given character. Only works with joined characters

---



<a class="header" id="property-change_character_mirror" href="#property-change_character_mirror">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_character_mirror</span>](#property-change_character_mirror) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `mirrored`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `force`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



Changes the mirror of the given character. Only works with joined characters

---



<a class="header" id="property-change_character_portrait" href="#property-change_character_portrait">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_character_portrait</span>](#property-change_character_portrait) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `update_transform`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span style = "color: gray">void</span>** 



Changes the portrait of a character. Only works with joined characters.

---



<a class="header" id="property-change_character_z_index" href="#property-change_character_z_index">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_character_z_index</span>](#property-change_character_z_index) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `z_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `update_zindex`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span style = "color: gray">void</span>** 



Changes the z_index of a character. Only works with joined characters

---



<a class="header" id="property-change_speaker" href="#property-change_speaker">**<span class="hljs-attribute">func</span> [<span class="hljs-title">change_speaker</span>](#property-change_speaker) ( `speaker`: [DialogicCharacter](class_dialogiccharacter.md) = `null`, `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



Updates all portrait containers set to SPEAKER.

---



<a class="header" id="property-clear_game_state" href="#property-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_character_info" href="#property-get_character_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_info</span>](#property-get_character_info) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Returns a dictionary with info on a given character. Keys can be [joined, character, node (for the portrait node), position_index] Only joined is included (and false) for not joined characters

---



<a class="header" id="property-get_joined_characters" href="#property-get_joined_characters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_joined_characters</span>](#property-get_joined_characters) ( )</a>  ⇒ <span class="hljs-attribute">[DialogicCharacter[]](https://docs.godotengine.org/en/latest/classes/class_dialogiccharacter.html#class-dialogiccharacter)</span>** 



Returns a list of the joined charcters (as resources)

---



<a class="header" id="property-get_portrait_container" href="#property-get_portrait_container">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_portrait_container</span>](#property-get_portrait_container) ( `postion_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-is_character_joined" href="#property-is_character_joined">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_character_joined</span>](#property-is_character_joined) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns true if the given character is currently joined.

---



<a class="header" id="property-join_character" href="#property-join_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">join_character</span>](#property-join_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `portrait`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `position_idx`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `mirrored`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `z_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0`, `extra_data`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



Adds a character at a position and sets it's portrait. If the character is already joined it will only update, portrait, position, etc.

---



<a class="header" id="property-leave_all_characters" href="#property-leave_all_characters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">leave_all_characters</span>](#property-leave_all_characters) ( `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



Removes all joined characters with a given animation or the default animation.

---



<a class="header" id="property-leave_character" href="#property-leave_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">leave_character</span>](#property-leave_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `animation_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `animation_length`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0`, `animation_wait`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



Removes a character with a given animation or the default animation.

---



<a class="header" id="property-load_game_state" href="#property-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#property-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-move_character" href="#property-move_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">move_character</span>](#property-move_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md), `position_idx`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Moves the given character to the given position. Only works with joined characters

---



<a class="header" id="property-move_portrait_position" href="#property-move_portrait_position">**<span class="hljs-attribute">func</span> [<span class="hljs-title">move_portrait_position</span>](#property-move_portrait_position) ( `position_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `vector`: [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2), `relative`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-pause" href="#property-pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">pause</span>](#property-pause) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-remove_character" href="#property-remove_character">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_character</span>](#property-remove_character) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Removes the given characters portrait. Only works with joined characters

---



<a class="header" id="property-reset_all_portrait_positions" href="#property-reset_all_portrait_positions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset_all_portrait_positions</span>](#property-reset_all_portrait_positions) ( `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-reset_portrait_position" href="#property-reset_portrait_position">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset_portrait_position</span>](#property-reset_portrait_position) ( `position_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `time`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `0.0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-resume" href="#property-resume">**<span class="hljs-attribute">func</span> [<span class="hljs-title">resume</span>](#property-resume) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text_effect_portrait" href="#property-text_effect_portrait">**<span class="hljs-attribute">func</span> [<span class="hljs-title">text_effect_portrait</span>](#property-text_effect_portrait) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Called from the [portrait=something] text effect.

---



<a class="header" id="property-z_sort_portrait_containers" href="#property-z_sort_portrait_containers">**<span class="hljs-attribute">func</span> [<span class="hljs-title">z_sort_portrait_containers</span>](#property-z_sort_portrait_containers) ( `con1`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md), `con2`: [DialogicNode_PortraitContainer](class_dialogicnode_portraitcontainer.md) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

