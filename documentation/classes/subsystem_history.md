
<div class="header-banner purple">
<div class="header-label purple">subsystem_History</div>
</div>

*This contains the source code documentation of the class `subsystem_History`.*
        
# subsystem_History
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that manages history storing.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">full_event_history_content</span>](#property-full_event_history_content) | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |   
[<span class="hljs-title">full_event_history_enabled</span>](#property-full_event_history_enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">save_visited_history_on_autosave</span>](#property-save_visited_history_on_autosave) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">save_visited_history_on_save</span>](#property-save_visited_history_on_save) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">simple_history_content</span>](#property-simple_history_content) | [Dictionary[]](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">simple_history_enabled</span>](#property-simple_history_enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">visited_event_history_content</span>](#property-visited_event_history_content) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">visited_event_history_enabled</span>](#property-visited_event_history_enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">visited_event_save_key</span>](#property-visited_event_save_key) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"visited_event_history_content"` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">close_history</span>](#property-close_history) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_saved_visited_history</span>](#property-get_saved_visited_history) ( ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_simple_history</span>](#property-get_simple_history) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_event_been_visited</span>](#property-has_event_been_visited) ( `event_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `<unknown>`, `timeline`: [DialogicTimeline](class_dialogictimeline.md) = `<unknown>` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_last_event_been_visited</span>](#property-has_last_event_been_visited) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">load_visited_history</span>](#property-load_visited_history) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">mark_event_as_visited</span>](#property-mark_event_as_visited) ( `_event`: [DialogicEvent](class_dialogicevent.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">open_history</span>](#property-open_history) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">post_install</span>](#property-post_install) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset_visited_history</span>](#property-reset_visited_history) ( `reset_property`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">save_visited_history</span>](#property-save_visited_history) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">store_full_event</span>](#property-store_full_event) ( `event`: [DialogicEvent](class_dialogicevent.md) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">store_simple_history_entry</span>](#property-store_simple_history_entry) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `event_type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` ) 
--- 

## Signals


<a class="header" id="signal-close_requested" href="#signal-close_requested">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">close_requested</span>](#signal-close_requested) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-full_event_history_changed" href="#signal-full_event_history_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">full_event_history_changed</span>](#signal-full_event_history_changed) ( )** </a>



Emitted if a new event has been inserted into the full event history.

---



<a class="header" id="signal-open_requested" href="#signal-open_requested">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">open_requested</span>](#signal-open_requested) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-simple_history_changed" href="#signal-simple_history_changed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">simple_history_changed</span>](#signal-simple_history_changed) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="signal-unvisited_event" href="#signal-unvisited_event">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">unvisited_event</span>](#signal-unvisited_event) ( )** </a>



Emitted if an encountered timeline event has not been visited before.

---



<a class="header" id="signal-visited_event" href="#signal-visited_event">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">visited_event</span>](#signal-visited_event) ( )** </a>



Emitted if an encountered timeline event has been inserted into the visited event history.  This will trigger only once per unique event instance.

---

## Property Descriptions



<a class="header" id="property-full_event_history_content" href="#property-full_event_history_content">**<span class="hljs-attribute">var</span> <span class="hljs-title">full_event_history_content</span> <span style = "color: gray"> = </span> <unknown>** 



The full history of all Dialogic events encountered. Requires `full_event_history_enabled` to be true.

---



<a class="header" id="property-full_event_history_enabled" href="#property-full_event_history_enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">full_event_history_enabled</span> <span style = "color: gray"> = </span> false** 



Whether to keep a history of every Dialogic event encountered.

---



<a class="header" id="property-save_visited_history_on_autosave" href="#property-save_visited_history_on_autosave">**<span class="hljs-attribute">var</span> <span class="hljs-title">save_visited_history_on_autosave</span> <span style = "color: gray"> = </span> false** 



Whether to automatically save the already-visited history on auto-save.

---



<a class="header" id="property-save_visited_history_on_save" href="#property-save_visited_history_on_save">**<span class="hljs-attribute">var</span> <span class="hljs-title">save_visited_history_on_save</span> <span style = "color: gray"> = </span> false** 



Whether to automatically save the already-visited history on manual save.

---



<a class="header" id="property-simple_history_content" href="#property-simple_history_content">**<span class="hljs-attribute">var</span> <span class="hljs-title">simple_history_content</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-simple_history_enabled" href="#property-simple_history_enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">simple_history_enabled</span> <span style = "color: gray"> = </span> true** 



Simple history that stores limited information Used for the history display

---



<a class="header" id="property-visited_event_history_content" href="#property-visited_event_history_content">**<span class="hljs-attribute">var</span> <span class="hljs-title">visited_event_history_content</span> <span style = "color: gray"> = </span> <unknown>** 



A history of visited Dialogic events.

---



<a class="header" id="property-visited_event_history_enabled" href="#property-visited_event_history_enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">visited_event_history_enabled</span> <span style = "color: gray"> = </span> false** 



Read text history Stores which text events and choices have already been visited

---



<a class="header" id="property-visited_event_save_key" href="#property-visited_event_save_key">**<span class="hljs-attribute">var</span> <span class="hljs-title">visited_event_save_key</span> <span style = "color: gray"> = </span> "visited_event_history_content"** 



Used to store `visited_event_history_content` in the global info file. You can change this to a custom name if you want to use a different key in the global save info file.

---

## Methods Descriptions



<a class="header" id="method-close_history" href="#method-close_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">close_history</span>](#property-close_history) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_saved_visited_history" href="#method-get_saved_visited_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_saved_visited_history</span>](#property-get_saved_visited_history) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Returns the saved already-visited history from the global info save file. If none exist in the global info file, returns an empty dictionary.  Relies on the [Save](subsystem_save.md) subsystem.

---



<a class="header" id="method-get_simple_history" href="#method-get_simple_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_simple_history</span>](#property-get_simple_history) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-has_event_been_visited" href="#method-has_event_been_visited">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_event_been_visited</span>](#property-has_event_been_visited) ( `event_index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `<unknown>`, `timeline`: [DialogicTimeline](class_dialogictimeline.md) = `<unknown>` )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



If called with with no arguments, the method will return whether the last encountered event was visited before.  Otherwise, if `event_index` and `timeline` are passed, the method will check if the event from that given timeline has been visited yet.  If no `timeline` is passed, the current timeline will be used. If there is no current timeline, `false` will be returned.  If no `event_index` is passed, the current event index will be used.

---



<a class="header" id="method-has_last_event_been_visited" href="#method-has_last_event_been_visited">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_last_event_been_visited</span>](#property-has_last_event_been_visited) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Whether the last event has been visited for the first time or not. This will return `true` exactly once for each unique timeline event instance.

---



<a class="header" id="method-load_visited_history" href="#method-load_visited_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">load_visited_history</span>](#property-load_visited_history) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Loads the seen events from the global info save file. Calling this when a game gets loaded may be useful.  Relies on the [Save](subsystem_save.md) subsystem.

---



<a class="header" id="method-mark_event_as_visited" href="#method-mark_event_as_visited">**<span class="hljs-attribute">func</span> [<span class="hljs-title">mark_event_as_visited</span>](#property-mark_event_as_visited) ( `_event`: [DialogicEvent](class_dialogicevent.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-open_history" href="#method-open_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">open_history</span>](#property-open_history) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-post_install" href="#method-post_install">**<span class="hljs-attribute">func</span> [<span class="hljs-title">post_install</span>](#property-post_install) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-reset_visited_history" href="#method-reset_visited_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset_visited_history</span>](#property-reset_visited_history) ( `reset_property`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) = `true` )</a>  ⇒ <span style = "color: gray">void</span>** 



Resets the already-visited history in the global info save file. If `reset_property` is true, it will also reset the already-visited history in the Dialogic Autoload.  Relies on the [Save](subsystem_save.md) subsystem.

---



<a class="header" id="method-save_visited_history" href="#method-save_visited_history">**<span class="hljs-attribute">func</span> [<span class="hljs-title">save_visited_history</span>](#property-save_visited_history) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Saves all seen events to the global info file. This can be useful when the player saves the game. In visual novels, callings this at the end of a route can be useful, as the player may not save the game.  Be aware, this won't add any events but completely overwrite the already saved ones.  Relies on the [Save](subsystem_save.md) subsystem.

---



<a class="header" id="method-store_full_event" href="#method-store_full_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">store_full_event</span>](#property-store_full_event) ( `event`: [DialogicEvent](class_dialogicevent.md) )</a>  ⇒ <span style = "color: gray">void</span>** 



Called on each event.

---



<a class="header" id="method-store_simple_history_entry" href="#method-store_simple_history_entry">**<span class="hljs-attribute">func</span> [<span class="hljs-title">store_simple_history_entry</span>](#property-store_simple_history_entry) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `event_type`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

