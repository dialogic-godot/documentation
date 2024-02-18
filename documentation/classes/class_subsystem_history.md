
<div class="header-banner purple">
<div class="header-label purple">subsystem_history</div>
</div>

*This contains the source code documentation of the class `subsystem_history`.*
        
# subsystem_history
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that manages history storing.
## Properties
Name | Type | Default 
--- | --- | --- 
already_read_history_content | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
already_read_history_enabled | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
already_seen_save_key | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"already_read_history_content"` 
full_event_history_content | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |   
full_event_history_enabled | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
simple_history_content | [Dictionary[]](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
simple_history_enabled | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">check_already_read</span>](#property-check_already_read) ( `event`: [DialogicEvent](class_dialogicevent.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">close_history</span>](#property-close_history) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">event_was_read</span>](#property-event_was_read) ( `_event`: [DialogicEvent](class_dialogicevent.md) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_saved_already_seen_history</span>](#property-get_saved_already_seen_history) ( ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_simple_history</span>](#property-get_simple_history) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_already_seen_history</span>](#property-load_already_seen_history) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">open_history</span>](#property-open_history) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">post_install</span>](#property-post_install) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset_already_seen_history</span>](#property-reset_already_seen_history) ( `reset_property`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">save_already_seen_history</span>](#property-save_already_seen_history) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">store_full_event</span>](#property-store_full_event) ( `event`: [DialogicEvent](class_dialogicevent.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">store_simple_history_entry</span>](#property-store_simple_history_entry) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `event_type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">was_last_event_already_read</span>](#property-was_last_event_already_read) ( ) 
--- 

## Signals


<a class="header" id="signal-already_read_event_reached" href="#signal-already_read_event_reached">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">already_read_event_reached</span>](#signal-already_read_event_reached) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-close_requested" href="#signal-close_requested">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">close_requested</span>](#signal-close_requested) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-full_event_history_changed" href="#signal-full_event_history_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">full_event_history_changed</span>](#signal-full_event_history_changed) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-not_read_event_reached" href="#signal-not_read_event_reached">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">not_read_event_reached</span>](#signal-not_read_event_reached) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-open_requested" href="#signal-open_requested">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">open_requested</span>](#signal-open_requested) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-simple_history_changed" href="#signal-simple_history_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">simple_history_changed</span>](#signal-simple_history_changed) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-check_already_read" href="#property-check_already_read">**<span class="hljs-attribute">func</span> [<span class="hljs-title">check_already_read</span>](#property-check_already_read) ( `event`: [DialogicEvent](class_dialogicevent.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-close_history" href="#property-close_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">close_history</span>](#property-close_history) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-event_was_read" href="#property-event_was_read">**<span class="hljs-attribute">func</span> [<span class="hljs-title">event_was_read</span>](#property-event_was_read) ( `_event`: [DialogicEvent](class_dialogicevent.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_saved_already_seen_history" href="#property-get_saved_already_seen_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_saved_already_seen_history</span>](#property-get_saved_already_seen_history) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Returns the saved already-seen history from the global info save file. If none exist in the global info file, returns an empty dictionary.  ## Relies on the Save subsystem.

---



<a class="header" id="property-get_simple_history" href="#property-get_simple_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_simple_history</span>](#property-get_simple_history) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-load_already_seen_history" href="#property-load_already_seen_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_already_seen_history</span>](#property-load_already_seen_history) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Loads the seen events from the global info save file. Calling this when a game gets loaded may be useful.  ## Relies on the Save subsystem.

---



<a class="header" id="property-open_history" href="#property-open_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">open_history</span>](#property-open_history) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-post_install" href="#property-post_install">**<span class="hljs-attribute">func</span> [<span class="hljs-title">post_install</span>](#property-post_install) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-reset_already_seen_history" href="#property-reset_already_seen_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset_already_seen_history</span>](#property-reset_already_seen_history) ( `reset_property`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) )</a>  ⇒ <span style = "color: gray">void</span>** 



Resets the already-seen history in the global info save file. If `reset_property` is true, it will also reset the already-seen history in the Dialogic Autoload.  ## Relies on the Save subsystem.

---



<a class="header" id="property-save_already_seen_history" href="#property-save_already_seen_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">save_already_seen_history</span>](#property-save_already_seen_history) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Saves all seen events to the global info file. This can be useful when the player saves the game. In visual novels, callings this at the end of a route can be useful, as the player may not save the game.  Be aware, this won't add any events but completely overwrite the already saved ones.  Relies on the Save subsystem.

---



<a class="header" id="property-store_full_event" href="#property-store_full_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">store_full_event</span>](#property-store_full_event) ( `event`: [DialogicEvent](class_dialogicevent.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Called on each event

---



<a class="header" id="property-store_simple_history_entry" href="#property-store_simple_history_entry">**<span class="hljs-attribute">func</span> [<span class="hljs-title">store_simple_history_entry</span>](#property-store_simple_history_entry) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `event_type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-was_last_event_already_read" href="#property-was_last_event_already_read">**<span class="hljs-attribute">func</span> [<span class="hljs-title">was_last_event_already_read</span>](#property-was_last_event_already_read) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

