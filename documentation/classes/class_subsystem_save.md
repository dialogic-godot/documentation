
<div class="header-banner purple">
<div class="header-label purple">subsystem_save</div>
</div>

*This contains the source code documentation of the class `subsystem_save`.*
        
# subsystem_save
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

# Subsystem that manages saving and loading data.
## Properties
Name | Type | Default 
--- | --- | --- 
autosave_timer | [Timer](https://docs.godotengine.org/en/latest/classes/class_timer.html#class-timer) |   
latest_thumbnail | [Image](https://docs.godotengine.org/en/latest/classes/class_image.html#class-image) |  `null` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_empty_slot</span>](#property-add_empty_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">delete_slot</span>](#property-delete_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_default_slot</span>](#property-get_default_slot) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_encryption_password</span>](#property-get_encryption_password) ( ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">get_global_info</span>](#property-get_global_info) ( `key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_latest_slot</span>](#property-get_latest_slot) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_slot_info</span>](#property-get_slot_info) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_slot_names</span>](#property-get_slot_names) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_slot_path</span>](#property-get_slot_path) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[ImageTexture](https://docs.godotengine.org/en/latest/classes/class_imagetexture.html#class-imagetexture)</span> | [<span class="hljs-title">get_slot_thumbnail</span>](#property-get_slot_thumbnail) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_slot</span>](#property-has_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load</span>](#property-load) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">load_file</span>](#property-load_file) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `file_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">perform_autosave</span>](#property-perform_autosave) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset_slot</span>](#property-reset_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">save</span>](#property-save) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `is_autosave`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `thumbnail_mode`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `1`, `slot_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">save_file</span>](#property-save_file) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `file_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `data`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">save_slot_thumbnail</span>](#property-save_slot_thumbnail) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_global_info</span>](#property-set_global_info) ( `key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_latest_slot</span>](#property-set_latest_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_slot_info</span>](#property-set_slot_info) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">take_thumbnail</span>](#property-take_thumbnail) ( ) 
--- 
## Constants


<a class="header" id="constant-SAVE_SLOTS_DIR" href="#constant-SAVE_SLOTS_DIR">**<span class="hljs-attribute">const</span> <span class="hljs-title">SAVE_SLOTS_DIR</span><span class="hljs-comment"> = "user://dialogic/saves/"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-NONE" href="#constant-NONE">**<span class="hljs-attribute">const</span> <span class="hljs-title">NONE</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-TAKE_AND_STORE" href="#constant-TAKE_AND_STORE">**<span class="hljs-attribute">const</span> <span class="hljs-title">TAKE_AND_STORE</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-STORE_ONLY" href="#constant-STORE_ONLY">**<span class="hljs-attribute">const</span> <span class="hljs-title">STORE_ONLY</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ON_TIMELINE_JUMPS" href="#constant-ON_TIMELINE_JUMPS">**<span class="hljs-attribute">const</span> <span class="hljs-title">ON_TIMELINE_JUMPS</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ON_TIMER" href="#constant-ON_TIMER">**<span class="hljs-attribute">const</span> <span class="hljs-title">ON_TIMER</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ON_TEXT_EVENT" href="#constant-ON_TEXT_EVENT">**<span class="hljs-attribute">const</span> <span class="hljs-title">ON_TEXT_EVENT</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-AUTO_SAVE_DEFAULT" href="#constant-AUTO_SAVE_DEFAULT">**<span class="hljs-attribute">const</span> <span class="hljs-title">AUTO_SAVE_DEFAULT</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-AUTO_SAVE_DEFAULT_DELAY" href="#constant-AUTO_SAVE_DEFAULT_DELAY">**<span class="hljs-attribute">const</span> <span class="hljs-title">AUTO_SAVE_DEFAULT_DELAY</span><span class="hljs-comment"> = 60</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-saved" href="#signal-saved">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">saved</span>](#signal-saved) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `is_autosave`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) )** </a>



Emitted when a save was done.

---

## Property Descriptions



<a class="header" id="property-add_empty_slot" href="#property-add_empty_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_empty_slot</span>](#property-add_empty_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



This adds a new save folder with the given name

---



<a class="header" id="property-clear_game_state" href="#property-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#property-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Built-in, called by DialogicGameHandler.

---



<a class="header" id="property-delete_slot" href="#property-delete_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">delete_slot</span>](#property-delete_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Removes all the given slot along with all it's info/files.

---



<a class="header" id="property-get_default_slot" href="#property-get_default_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_default_slot</span>](#property-get_default_slot) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the default slot name defined in the dialogic settings

---



<a class="header" id="property-get_encryption_password" href="#property-get_encryption_password">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_encryption_password</span>](#property-get_encryption_password) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Gets the encryption password from the project settings if it has been set. If no password has been set, an empty string is returned.

---



<a class="header" id="property-get_global_info" href="#property-get_global_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_global_info</span>](#property-get_global_info) ( `key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



Access the data unrelated to a save slot. First, the data must have been set with [set_global_info](#property-set_global_info).

---



<a class="header" id="property-get_latest_slot" href="#property-get_latest_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_latest_slot</span>](#property-get_latest_slot) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the latest slot or empty if nothing was saved yet

---



<a class="header" id="property-get_slot_info" href="#property-get_slot_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_slot_info</span>](#property-get_slot_info) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_slot_names" href="#property-get_slot_names">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_slot_names</span>](#property-get_slot_names) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



################################################################################################## Returns a list of all available slots. Useful for iterating over all slots, e.g., when building a UI with all save slots.

---



<a class="header" id="property-get_slot_path" href="#property-get_slot_path">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_slot_path</span>](#property-get_slot_path) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the full path to the given slot folder

---



<a class="header" id="property-get_slot_thumbnail" href="#property-get_slot_thumbnail">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_slot_thumbnail</span>](#property-get_slot_thumbnail) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[ImageTexture](https://docs.godotengine.org/en/latest/classes/class_imagetexture.html#class-imagetexture)</span>** 



Returns the thumbnail of the given slot.

---



<a class="header" id="property-has_slot" href="#property-has_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_slot</span>](#property-has_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns true if the given slot exists.

---



<a class="header" id="property-load" href="#property-load">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load</span>](#property-load) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



Loads all info from the given slot in the DialogicGameHandler (Dialogic Autoload). If no slot is given, the default slot is used. To check if something is saved in that slot use has_slot(). If the slot does not exist, this method will fail.

---



<a class="header" id="property-load_file" href="#property-load_file">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_file</span>](#property-load_file) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `file_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



Loads a file from a given list and returns the contained info as a variable.

---



<a class="header" id="property-perform_autosave" href="#property-perform_autosave">**<span class="hljs-attribute">func</span> [<span class="hljs-title">perform_autosave</span>](#property-perform_autosave) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Perform an autosave. This method will be called automatically if the auto-save mode is enabled.

---



<a class="header" id="property-reset_slot" href="#property-reset_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset_slot</span>](#property-reset_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



Reset the state of the given save folder (or default)

---



<a class="header" id="property-save" href="#property-save">**<span class="hljs-attribute">func</span> [<span class="hljs-title">save</span>](#property-save) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""`, `is_autosave`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `false`, `thumbnail_mode`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `1`, `slot_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` )</a>  ⇒ <span style = "color: gray">void</span>** 



Saves the current state to the given slot. If no slot is given, the default slot is used. You can change this name in the Dialogic editor. If you want to save to the last used slot, you can get its slot name with the [get_latest_slot()](#property-get_latest_slot()) method.

---



<a class="header" id="property-save_file" href="#property-save_file">**<span class="hljs-attribute">func</span> [<span class="hljs-title">save_file</span>](#property-save_file) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `file_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `data`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span style = "color: gray">void</span>** 



Saves a variable to a file in the given slot.  Be aware, the `slot_name` will be used a filesystem folder name. Some operating systems do not support every character in folder names. It is recommended to use only letters, numbers, and underscores.

---



<a class="header" id="property-save_slot_thumbnail" href="#property-save_slot_thumbnail">**<span class="hljs-attribute">func</span> [<span class="hljs-title">save_slot_thumbnail</span>](#property-save_slot_thumbnail) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



No need to call from outside. Used to store the latest thumbnail to the given slot.

---



<a class="header" id="property-set_global_info" href="#property-set_global_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_global_info</span>](#property-set_global_info) ( `key`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span style = "color: gray">void</span>** 



Data set in global info can be accessed unrelated to the save slots. Information such as the player name can be saved here.

---



<a class="header" id="property-set_latest_slot" href="#property-set_latest_slot">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_latest_slot</span>](#property-set_latest_slot) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_slot_info" href="#property-set_slot_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_slot_info</span>](#property-set_slot_info) ( `slot_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-take_thumbnail" href="#property-take_thumbnail">**<span class="hljs-attribute">func</span> [<span class="hljs-title">take_thumbnail</span>](#property-take_thumbnail) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Can be called manually to create a thumbnail. Then, call [save](#property-save) with ThumbnailMode.STORE_ONLY to save the game use the thumbnail prepared with this method.

---

