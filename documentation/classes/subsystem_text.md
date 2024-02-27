
<div class="header-banner purple">
<div class="header-label purple">subsystem_Text</div>
</div>

*This contains the source code documentation of the class `subsystem_Text`.*
        
# subsystem_Text
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that handles showing of dialog text (+text effects & modifiers), name label, and next indicator
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">character_colors</span>](#property-character_colors) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">color_regex</span>](#property-color_regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
[<span class="hljs-title">modifier_words_select_regex</span>](#property-modifier_words_select_regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
[<span class="hljs-title">parsed_text_effect_info</span>](#property-parsed_text_effect_info) | [Dictionary[]](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">text_already_read</span>](#property-text_already_read) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">text_effects</span>](#property-text_effects) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">text_effects_regex</span>](#property-text_effects_regex) | [RegEx](https://docs.godotengine.org/en/latest/classes/class_regex.html#class-regex) |   
[<span class="hljs-title">text_modifiers</span>](#property-text_modifiers) | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">collect_character_names</span>](#property-collect_character_names) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">collect_text_effects</span>](#property-collect_text_effects) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">collect_text_modifiers</span>](#property-collect_text_modifiers) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">color_names</span>](#property-color_names) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">connect_meta_signals</span>](#property-connect_meta_signals) ( `text_node`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_lspeed</span>](#property-effect_lspeed) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_mood</span>](#property-effect_mood) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_pause</span>](#property-effect_pause) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_signal</span>](#property-effect_signal) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">effect_speed</span>](#property-effect_speed) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">emit_meta_signal</span>](#property-emit_meta_signal) ( `meta`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `sig`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">execute_effects</span>](#property-execute_effects) ( `current_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipping`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">[DialogicCharacter](class_dialogiccharacter.md)</span> | [<span class="hljs-title">get_current_speaker</span>](#property-get_current_speaker) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">hide_next_indicators</span>](#property-hide_next_indicators) ( `_fake_arg`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">hide_textbox</span>](#property-hide_textbox) ( `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_text_reveal_skippable</span>](#property-is_text_reveal_skippable) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_text_voice_synced</span>](#property-is_text_voice_synced) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_textbox_visible</span>](#property-is_textbox_visible) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_game_state</span>](#property-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">modifier_autopauses</span>](#property-modifier_autopauses) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">modifier_break</span>](#property-modifier_break) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">modifier_random_selection</span>](#property-modifier_random_selection) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">parse_text</span>](#property-parse_text) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0`, `variables`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `glossary`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `modifiers`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `effects`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `color_names`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">parse_text_effects</span>](#property-parse_text_effects) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">parse_text_modifiers</span>](#property-parse_text_modifiers) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">post_install</span>](#property-post_install) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_text_reveal_skippable</span>](#property-set_text_reveal_skippable) ( `skippable`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `temp`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_text_voice_synced</span>](#property-set_text_voice_synced) ( `enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">show_next_indicators</span>](#property-show_next_indicators) ( `question`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `autoadvance`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">show_textbox</span>](#property-show_textbox) ( `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">skip_text_reveal</span>](#property-skip_text_reveal) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">update_dialog_text</span>](#property-update_dialog_text) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `additional`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_name_label</span>](#property-update_name_label) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_text_speed</span>](#property-update_text_speed) ( `letter_speed`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `-1.0`, `absolute`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `speed_multiplier`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `<unknown>`, `user_speed`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `<unknown>` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_textbox</span>](#property-update_textbox) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_typing_sound_mood</span>](#property-update_typing_sound_mood) ( `mood`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` ) 
--- 
## Constants


<a class="header" id="constant-ALL" href="#constant-ALL">**<span class="hljs-attribute">const</span> <span class="hljs-title">ALL</span><span class="hljs-comment"> = -1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TEXT_ONLY" href="#constant-TEXT_ONLY">**<span class="hljs-attribute">const</span> <span class="hljs-title">TEXT_ONLY</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-CHOICES_ONLY" href="#constant-CHOICES_ONLY">**<span class="hljs-attribute">const</span> <span class="hljs-title">CHOICES_ONLY</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-DIALOG_TEXT" href="#constant-DIALOG_TEXT">**<span class="hljs-attribute">const</span> <span class="hljs-title">DIALOG_TEXT</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-CHOICE_TEXT" href="#constant-CHOICE_TEXT">**<span class="hljs-attribute">const</span> <span class="hljs-title">CHOICE_TEXT</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-about_to_show_text" href="#signal-about_to_show_text">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">about_to_show_text</span>](#signal-about_to_show_text) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-animation_textbox_hide" href="#signal-animation_textbox_hide">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">animation_textbox_hide</span>](#signal-animation_textbox_hide) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-animation_textbox_new_text" href="#signal-animation_textbox_new_text">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">animation_textbox_new_text</span>](#signal-animation_textbox_new_text) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-animation_textbox_show" href="#signal-animation_textbox_show">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">animation_textbox_show</span>](#signal-animation_textbox_show) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-meta_clicked" href="#signal-meta_clicked">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">meta_clicked</span>](#signal-meta_clicked) ( `meta`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-meta_hover_ended" href="#signal-meta_hover_ended">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">meta_hover_ended</span>](#signal-meta_hover_ended) ( `meta`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-meta_hover_started" href="#signal-meta_hover_started">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">meta_hover_started</span>](#signal-meta_hover_started) ( `meta`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-speaker_updated" href="#signal-speaker_updated">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">speaker_updated</span>](#signal-speaker_updated) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-text_finished" href="#signal-text_finished">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">text_finished</span>](#signal-text_finished) ( `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-textbox_visibility_changed" href="#signal-textbox_visibility_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">textbox_visibility_changed</span>](#signal-textbox_visibility_changed) ( `visible`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-character_colors" href="#property-character_colors">**<span class="hljs-attribute">var</span> <span class="hljs-title">character_colors</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-color_regex" href="#property-color_regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">color_regex</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-modifier_words_select_regex" href="#property-modifier_words_select_regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">modifier_words_select_regex</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-parsed_text_effect_info" href="#property-parsed_text_effect_info">**<span class="hljs-attribute">var</span> <span class="hljs-title">parsed_text_effect_info</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text_already_read" href="#property-text_already_read">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_already_read</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text_effects" href="#property-text_effects">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_effects</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text_effects_regex" href="#property-text_effects_regex">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_effects_regex</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text_modifiers" href="#property-text_modifiers">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_modifiers</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---

## Methods Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-collect_character_names" href="#method-collect_character_names">**<span class="hljs-attribute">func</span> [<span class="hljs-title">collect_character_names</span>](#property-collect_character_names) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-collect_text_effects" href="#method-collect_text_effects">**<span class="hljs-attribute">func</span> [<span class="hljs-title">collect_text_effects</span>](#property-collect_text_effects) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-collect_text_modifiers" href="#method-collect_text_modifiers">**<span class="hljs-attribute">func</span> [<span class="hljs-title">collect_text_modifiers</span>](#property-collect_text_modifiers) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-color_names" href="#method-color_names">**<span class="hljs-attribute">func</span> [<span class="hljs-title">color_names</span>](#property-color_names) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-connect_meta_signals" href="#method-connect_meta_signals">**<span class="hljs-attribute">func</span> [<span class="hljs-title">connect_meta_signals</span>](#property-connect_meta_signals) ( `text_node`: [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-effect_lspeed" href="#method-effect_lspeed">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_lspeed</span>](#property-effect_lspeed) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-effect_mood" href="#method-effect_mood">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_mood</span>](#property-effect_mood) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-effect_pause" href="#method-effect_pause">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_pause</span>](#property-effect_pause) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-effect_signal" href="#method-effect_signal">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_signal</span>](#property-effect_signal) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-effect_speed" href="#method-effect_speed">**<span class="hljs-attribute">func</span> [<span class="hljs-title">effect_speed</span>](#property-effect_speed) ( `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipped`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool), `argument`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-emit_meta_signal" href="#method-emit_meta_signal">**<span class="hljs-attribute">func</span> [<span class="hljs-title">emit_meta_signal</span>](#property-emit_meta_signal) ( `meta`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant), `sig`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-execute_effects" href="#method-execute_effects">**<span class="hljs-attribute">func</span> [<span class="hljs-title">execute_effects</span>](#property-execute_effects) ( `current_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int), `text_node`: [Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control), `skipping`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_current_speaker" href="#method-get_current_speaker">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_current_speaker</span>](#property-get_current_speaker) ( )</a>  ⇒ <span class="hljs-attribute">[DialogicCharacter](class_dialogiccharacter.md)</span>** 



Returns the [DialogicCharacter](class_dialogiccharacter.md) of the current speaker. If there is no current speaker or the speaker is not found, returns null.

---



<a class="header" id="method-hide_next_indicators" href="#method-hide_next_indicators">**<span class="hljs-attribute">func</span> [<span class="hljs-title">hide_next_indicators</span>](#property-hide_next_indicators) ( `_fake_arg`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-hide_textbox" href="#method-hide_textbox">**<span class="hljs-attribute">func</span> [<span class="hljs-title">hide_textbox</span>](#property-hide_textbox) ( `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



Instant skips the signal and thus possible animations

---



<a class="header" id="method-is_text_reveal_skippable" href="#method-is_text_reveal_skippable">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_text_reveal_skippable</span>](#property-is_text_reveal_skippable) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_text_voice_synced" href="#method-is_text_voice_synced">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_text_voice_synced</span>](#property-is_text_voice_synced) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns whether voice-synced text is enabled.

---



<a class="header" id="method-is_textbox_visible" href="#method-is_textbox_visible">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_textbox_visible</span>](#property-is_textbox_visible) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-load_game_state" href="#method-load_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_game_state</span>](#property-load_game_state) ( `load_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-modifier_autopauses" href="#method-modifier_autopauses">**<span class="hljs-attribute">func</span> [<span class="hljs-title">modifier_autopauses</span>](#property-modifier_autopauses) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-modifier_break" href="#method-modifier_break">**<span class="hljs-attribute">func</span> [<span class="hljs-title">modifier_break</span>](#property-modifier_break) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-modifier_random_selection" href="#method-modifier_random_selection">**<span class="hljs-attribute">func</span> [<span class="hljs-title">modifier_random_selection</span>](#property-modifier_random_selection) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-parse_text" href="#method-parse_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">parse_text</span>](#property-parse_text) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0`, `variables`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `glossary`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `modifiers`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `effects`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `color_names`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Applies modifiers, effects and coloring to the text

---



<a class="header" id="method-parse_text_effects" href="#method-parse_text_effects">**<span class="hljs-attribute">func</span> [<span class="hljs-title">parse_text_effects</span>](#property-parse_text_effects) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the string with all text effects removed Use get_parsed_text_effects() after calling this to get all effect information

---



<a class="header" id="method-parse_text_modifiers" href="#method-parse_text_modifiers">**<span class="hljs-attribute">func</span> [<span class="hljs-title">parse_text_modifiers</span>](#property-parse_text_modifiers) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-post_install" href="#method-post_install">**<span class="hljs-attribute">func</span> [<span class="hljs-title">post_install</span>](#property-post_install) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_text_reveal_skippable" href="#method-set_text_reveal_skippable">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_text_reveal_skippable</span>](#property-set_text_reveal_skippable) ( `skippable`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true`, `temp`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_text_voice_synced" href="#method-set_text_voice_synced">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_text_voice_synced</span>](#property-set_text_voice_synced) ( `enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span style = "color: gray">void</span>** 



This method will sync the text speed to the voice audio clip length, if a voice is playing. For instance, if the voice is playing for four seconds, the text will finish revealing after this time. This feature ignores Auto-Pauses on letters. Pauses via BBCode will desync the reveal.

---



<a class="header" id="method-show_next_indicators" href="#method-show_next_indicators">**<span class="hljs-attribute">func</span> [<span class="hljs-title">show_next_indicators</span>](#property-show_next_indicators) ( `question`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `autoadvance`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-show_textbox" href="#method-show_textbox">**<span class="hljs-attribute">func</span> [<span class="hljs-title">show_textbox</span>](#property-show_textbox) ( `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



instant skips the signal and thus possible animations

---



<a class="header" id="method-skip_text_reveal" href="#method-skip_text_reveal">**<span class="hljs-attribute">func</span> [<span class="hljs-title">skip_text_reveal</span>](#property-skip_text_reveal) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-update_dialog_text" href="#method-update_dialog_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_dialog_text</span>](#property-update_dialog_text) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `additional`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Shows the given text on all visible DialogText nodes. Instant can be used to skip all revieling. If additional is true, the previous text will be kept.

---



<a class="header" id="method-update_name_label" href="#method-update_name_label">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_name_label</span>](#property-update_name_label) ( `character`: [DialogicCharacter](class_dialogiccharacter.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Updates the visible name on all name labels nodes. If a name changes, the [speaker_updated](#signal-speaker_updated) signal is emitted.

---



<a class="header" id="method-update_text_speed" href="#method-update_text_speed">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_text_speed</span>](#property-update_text_speed) ( `letter_speed`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `-1.0`, `absolute`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `speed_multiplier`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `<unknown>`, `user_speed`: [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) = `<unknown>` )</a>  ⇒ <span style = "color: gray">void</span>** 



Sets how fast text will be revealed.  `absolute` will force test to display at the given speed, regardless of the user's text speed setting.  `_speed_multiplier` adjusts the speed of the text, if set to -1, the value won't be updated and the current value will persist.  `_user_speed` adjusts the speed of the text, if set to -1, the project setting 'text_speed' will be used.operator

---



<a class="header" id="method-update_textbox" href="#method-update_textbox">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_textbox</span>](#property-update_textbox) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `instant`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false` )</a>  ⇒ <span style = "color: gray">void</span>** 



When an event updates the text spoken, this can adjust the state of the dialog text box. This method is async.

---



<a class="header" id="method-update_typing_sound_mood" href="#method-update_typing_sound_mood">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_typing_sound_mood</span>](#property-update_typing_sound_mood) ( `mood`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

