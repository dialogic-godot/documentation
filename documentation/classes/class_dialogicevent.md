
<div class="header-banner purple">
<div class="header-label purple">DialogicEvent</div>
</div>

*This contains the source code documentation of the class `DialogicEvent`.*
        
# DialogicEvent
**Inherits:** [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource)

Base event class for all dialogic events. Implements basic properties, translation, shortcode saving and usefull methods for creating the editor UI.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">can_contain_events</span>](#property-can_contain_events) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">created_by_button</span>](#property-created_by_button) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">dialogic</span>](#property-dialogic) | [DialogicGameHandler](class_dialogicgamehandler.md) |  `null` 
[<span class="hljs-title">dialogic_color_name</span>](#property-dialogic_color_name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">disable_editor_button</span>](#property-disable_editor_button) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">display_name</span>](#property-display_name) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
[<span class="hljs-title">editor_list</span>](#property-editor_list) | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |   
[<span class="hljs-title">empty_lines_above</span>](#property-empty_lines_above) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">end_branch_event</span>](#property-end_branch_event) | [DialogicEndBranchEvent](class_dialogicendbranchevent.md) |  `null` 
[<span class="hljs-title">event_category</span>](#property-event_category) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"Other"` 
[<span class="hljs-title">event_color</span>](#property-event_color) | [Color](https://docs.godotengine.org/en/latest/classes/class_color.html#class-color) |  `Color(0.984314, 0.694118, 0.235294, 1)` 
[<span class="hljs-title">event_name</span>](#property-event_name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"Event"` 
[<span class="hljs-title">event_node_as_text</span>](#property-event_node_as_text) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">event_node_ready</span>](#property-event_node_ready) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">event_sorting_index</span>](#property-event_sorting_index) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">expand_by_default</span>](#property-expand_by_default) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">help_page_path</span>](#property-help_page_path) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">needs_indentation</span>](#property-needs_indentation) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">wants_to_group</span>](#property-wants_to_group) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_body_edit</span>](#method-add_body_edit) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `editor_type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `16`, `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_body_line_break</span>](#method-add_body_line_break) ( `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_header_button</span>](#method-add_header_button) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `callable`: [Callable](https://docs.godotengine.org/en/latest/classes/class_callable.html#class-callable), `tooltip`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `icon`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_header_edit</span>](#method-add_header_edit) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `editor_type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `16`, `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">add_header_label</span>](#method-add_header_label) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">add_translation_id</span>](#method-add_translation_id) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">can_be_translated</span>](#method-can_be_translated) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">execute</span>](#method-execute) ( `_dialogic_game_handler`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">finish</span>](#method-finish) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)</span> | [<span class="hljs-title">get_end_branch_control</span>](#method-get_end_branch_control) ( ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_event_editor_info</span>](#method-get_event_editor_info) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_property_translated</span>](#method-get_property_translated) ( `property_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_property_translation_key</span>](#method-get_property_translation_key) ( `property_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_shortcode</span>](#method-get_shortcode) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_string_full_event</span>](#method-is_string_full_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">parse_shortcode_parameters</span>](#method-parse_shortcode_parameters) ( `shortcode`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">remove_translation_id</span>](#method-remove_translation_id) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">set_default_color</span>](#method-set_default_color) ( `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">should_execute_this_branch</span>](#method-should_execute_this_branch) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">to_text</span>](#method-to_text) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">update_text_version</span>](#method-update_text_version) ( ) 
--- 
## Constants


<a class="header" id="constant-HEADER" href="#constant-HEADER">**<span class="hljs-attribute">const</span> <span class="hljs-title">HEADER</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-BODY" href="#constant-BODY">**<span class="hljs-attribute">const</span> <span class="hljs-title">BODY</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-MULTILINE_TEXT" href="#constant-MULTILINE_TEXT">**<span class="hljs-attribute">const</span> <span class="hljs-title">MULTILINE_TEXT</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-SINGLELINE_TEXT" href="#constant-SINGLELINE_TEXT">**<span class="hljs-attribute">const</span> <span class="hljs-title">SINGLELINE_TEXT</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-CONDITION" href="#constant-CONDITION">**<span class="hljs-attribute">const</span> <span class="hljs-title">CONDITION</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-FILE" href="#constant-FILE">**<span class="hljs-attribute">const</span> <span class="hljs-title">FILE</span><span class="hljs-comment"> = 3</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-BOOL" href="#constant-BOOL">**<span class="hljs-attribute">const</span> <span class="hljs-title">BOOL</span><span class="hljs-comment"> = 4</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-BOOL_BUTTON" href="#constant-BOOL_BUTTON">**<span class="hljs-attribute">const</span> <span class="hljs-title">BOOL_BUTTON</span><span class="hljs-comment"> = 5</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-DYNAMIC_OPTIONS" href="#constant-DYNAMIC_OPTIONS">**<span class="hljs-attribute">const</span> <span class="hljs-title">DYNAMIC_OPTIONS</span><span class="hljs-comment"> = 6</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-FIXED_OPTIONS" href="#constant-FIXED_OPTIONS">**<span class="hljs-attribute">const</span> <span class="hljs-title">FIXED_OPTIONS</span><span class="hljs-comment"> = 7</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ARRAY" href="#constant-ARRAY">**<span class="hljs-attribute">const</span> <span class="hljs-title">ARRAY</span><span class="hljs-comment"> = 8</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-DICTIONARY" href="#constant-DICTIONARY">**<span class="hljs-attribute">const</span> <span class="hljs-title">DICTIONARY</span><span class="hljs-comment"> = 9</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-NUMBER" href="#constant-NUMBER">**<span class="hljs-attribute">const</span> <span class="hljs-title">NUMBER</span><span class="hljs-comment"> = 10</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-VECTOR2" href="#constant-VECTOR2">**<span class="hljs-attribute">const</span> <span class="hljs-title">VECTOR2</span><span class="hljs-comment"> = 11</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-VECTOR3" href="#constant-VECTOR3">**<span class="hljs-attribute">const</span> <span class="hljs-title">VECTOR3</span><span class="hljs-comment"> = 12</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-VECTOR4" href="#constant-VECTOR4">**<span class="hljs-attribute">const</span> <span class="hljs-title">VECTOR4</span><span class="hljs-comment"> = 13</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-CUSTOM" href="#constant-CUSTOM">**<span class="hljs-attribute">const</span> <span class="hljs-title">CUSTOM</span><span class="hljs-comment"> = 14</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-BUTTON" href="#constant-BUTTON">**<span class="hljs-attribute">const</span> <span class="hljs-title">BUTTON</span><span class="hljs-comment"> = 15</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-LABEL" href="#constant-LABEL">**<span class="hljs-attribute">const</span> <span class="hljs-title">LABEL</span><span class="hljs-comment"> = 16</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-event_finished" href="#signal-event_finished">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">event_finished</span>](#signal-event_finished) ( `event_resource`: [DialogicEvent](class_dialogicevent.md) )** </a>



 Emmited when the event finish. The signal is emmited with the event resource event_resource[/code] 

---



<a class="header" id="signal-event_started" href="#signal-event_started">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">event_started</span>](#signal-event_started) ( `event_resource`: [DialogicEvent](class_dialogicevent.md) )** </a>



 Emmited when the event starts. The signal is emmited with the event resource event_resource[/code] 

---



<a class="header" id="signal-ui_update_needed" href="#signal-ui_update_needed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">ui_update_needed</span>](#signal-ui_update_needed) ( )** </a>



 Singal that notifies the visual editor block to update 

---



<a class="header" id="signal-ui_update_warning" href="#signal-ui_update_warning">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">ui_update_warning</span>](#signal-ui_update_warning) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-can_contain_events" href="#property-can_contain_events">**<span class="hljs-attribute">var</span> <span class="hljs-title">can_contain_events</span> <span style = "color: gray"> = </span> false** 



If true this event will spawn with an END BRANCH event and higher the indentation

---



<a class="header" id="property-created_by_button" href="#property-created_by_button">**<span class="hljs-attribute">var</span> <span class="hljs-title">created_by_button</span> <span style = "color: gray"> = </span> false** 



Is the event block created by a button?

---



<a class="header" id="property-dialogic" href="#property-dialogic">**<span class="hljs-attribute">var</span> <span class="hljs-title">dialogic</span> <span style = "color: gray"> = </span> null** 



A reference to dialogic during execution, can be used the same as Dialogic (reference to the autoload)

---



<a class="header" id="property-dialogic_color_name" href="#property-dialogic_color_name">**<span class="hljs-attribute">var</span> <span class="hljs-title">dialogic_color_name</span> <span style = "color: gray"> = </span> ""** 



If you are using the default color palette

---



<a class="header" id="property-disable_editor_button" href="#property-disable_editor_button">**<span class="hljs-attribute">var</span> <span class="hljs-title">disable_editor_button</span> <span style = "color: gray"> = </span> false** 



If true the event will not have a button in the visual editor sidebar

---



<a class="header" id="property-display_name" href="#property-display_name">**<span class="hljs-attribute">var</span> <span class="hljs-title">display_name</span> <span style = "color: gray"> = </span> true** 



If false the name is not displayed on the event.

---



<a class="header" id="property-editor_list" href="#property-editor_list">**<span class="hljs-attribute">var</span> <span class="hljs-title">editor_list</span> <span style = "color: gray"> = </span> <unknown>** 



List that stores the fields for the editor

---



<a class="header" id="property-empty_lines_above" href="#property-empty_lines_above">**<span class="hljs-attribute">var</span> <span class="hljs-title">empty_lines_above</span> <span style = "color: gray"> = </span> 0** 



How many empty lines are before this event

---



<a class="header" id="property-end_branch_event" href="#property-end_branch_event">**<span class="hljs-attribute">var</span> <span class="hljs-title">end_branch_event</span> <span style = "color: gray"> = </span> null** 



If  is true this is a reference to the end branch event

---



<a class="header" id="property-event_category" href="#property-event_category">**<span class="hljs-attribute">var</span> <span class="hljs-title">event_category</span> <span style = "color: gray"> = </span> "Other"** 



The categories and which one to put it in (in the visual editor sidebar)

---



<a class="header" id="property-event_color" href="#property-event_color">**<span class="hljs-attribute">var</span> <span class="hljs-title">event_color</span> <span style = "color: gray"> = </span> Color(0.984314, 0.694118, 0.235294, 1)** 



The event color that event node will take in the editor

---



<a class="header" id="property-event_name" href="#property-event_name">**<span class="hljs-attribute">var</span> <span class="hljs-title">event_name</span> <span style = "color: gray"> = </span> "Event"** 



The event name that'll be displayed in the editor.

---



<a class="header" id="property-event_node_as_text" href="#property-event_node_as_text">**<span class="hljs-attribute">var</span> <span class="hljs-title">event_node_as_text</span> <span style = "color: gray"> = </span> ""** 



Stores the event in a text format. Does NOT automatically update.

---



<a class="header" id="property-event_node_ready" href="#property-event_node_ready">**<span class="hljs-attribute">var</span> <span class="hljs-title">event_node_ready</span> <span style = "color: gray"> = </span> false** 



Flags if the event has been processed or is only stored as text

---



<a class="header" id="property-event_sorting_index" href="#property-event_sorting_index">**<span class="hljs-attribute">var</span> <span class="hljs-title">event_sorting_index</span> <span style = "color: gray"> = </span> 0** 



To sort the buttons shown in the editor. Lower index is placed at the top of a category

---



<a class="header" id="property-expand_by_default" href="#property-expand_by_default">**<span class="hljs-attribute">var</span> <span class="hljs-title">expand_by_default</span> <span style = "color: gray"> = </span> false** 



If false the event will hide it's body by default. Recommended for most events

---



<a class="header" id="property-help_page_path" href="#property-help_page_path">**<span class="hljs-attribute">var</span> <span class="hljs-title">help_page_path</span> <span style = "color: gray"> = </span> ""** 



The URL to open when right_click>Documentation is selected

---



<a class="header" id="property-needs_indentation" href="#property-needs_indentation">**<span class="hljs-attribute">var</span> <span class="hljs-title">needs_indentation</span> <span style = "color: gray"> = </span> false** 



If true this event can not be toplevel (e.g. Choice)

---



<a class="header" id="property-wants_to_group" href="#property-wants_to_group">**<span class="hljs-attribute">var</span> <span class="hljs-title">wants_to_group</span> <span style = "color: gray"> = </span> false** 



If this is true this event will group with other similar events (like choices do).

---

## Method Descriptions



<a class="header" id="method-add_body_edit" href="#method-add_body_edit">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_body_edit</span>](#method-add_body_edit) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `editor_type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `16`, `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-add_body_line_break" href="#method-add_body_line_break">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_body_line_break</span>](#method-add_body_line_break) ( `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-add_header_button" href="#method-add_header_button">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_header_button</span>](#method-add_header_button) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `callable`: [Callable](https://docs.godotengine.org/en/latest/classes/class_callable.html#class-callable), `tooltip`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `icon`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-add_header_edit" href="#method-add_header_edit">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_header_edit</span>](#method-add_header_edit) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `editor_type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `16`, `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-add_header_label" href="#method-add_header_label">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_header_label</span>](#method-add_header_label) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-add_translation_id" href="#method-add_translation_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_translation_id</span>](#method-add_translation_id) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



This is automatically called, no need to use this.

---



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



to be overwritten by the sub_classes

---



<a class="header" id="method-can_be_translated" href="#method-can_be_translated">**<span class="hljs-attribute">func</span> [<span class="hljs-title">can_be_translated</span>](#method-can_be_translated) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Returns true if there is any translatable properties on this event. Overwrite [_get_translatable_properties()] to change this.

---



<a class="header" id="method-execute" href="#method-execute">**<span class="hljs-attribute">func</span> [<span class="hljs-title">execute</span>](#method-execute) ( `_dialogic_game_handler`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span style = "color: gray">void</span>** 



Executes the event behaviour. In subclasses  (not this one) should be overriden!

---



<a class="header" id="method-finish" href="#method-finish">**<span class="hljs-attribute">func</span> [<span class="hljs-title">finish</span>](#method-finish) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Ends the event behaviour.

---



<a class="header" id="method-from_text" href="#method-from_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



loads the variables from the string stored above by default it uses the shortcode format, but can be overridden

---



<a class="header" id="method-get_end_branch_control" href="#method-get_end_branch_control">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_end_branch_control</span>](#method-get_end_branch_control) ( )</a>  ⇒ <span class="hljs-attribute">[Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)</span>** 



to be overridden by sub-classes only called if can_contain_events is true. return a control node that should show on the END BRANCH node

---



<a class="header" id="method-get_event_editor_info" href="#method-get_event_editor_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_event_editor_info</span>](#method-get_event_editor_info) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_property_translated" href="#method-get_property_translated">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_property_translated</span>](#method-get_property_translated) ( `property_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Call this whenever you are using a translatable property

---



<a class="header" id="method-get_property_translation_key" href="#method-get_property_translation_key">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_property_translation_key</span>](#method-get_property_translation_key) ( `property_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode" href="#method-get_shortcode">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode</span>](#method-get_shortcode) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



if this uses the short-code format, return the shortcode

---



<a class="header" id="method-get_shortcode_parameters" href="#method-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



if this uses the short-code format, return the parameters and corresponding property names

---



<a class="header" id="method-is_string_full_event" href="#method-is_string_full_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_string_full_event</span>](#method-is_string_full_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



has to return true if this string seems to be a full event of this kind (only tested if is_valid_event() returned true) if a shortcode it used it will default to true if the string ends with ']'

---



<a class="header" id="method-is_valid_event" href="#method-is_valid_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



has to return true, if the given string can be interpreted as this event by default it uses the shortcode formta, but can be overridden

---



<a class="header" id="method-parse_shortcode_parameters" href="#method-parse_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">parse_shortcode_parameters</span>](#method-parse_shortcode_parameters) ( `shortcode`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



used to get all the shortcode parameters in a string as a dictionary

---



<a class="header" id="method-remove_translation_id" href="#method-remove_translation_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_translation_id</span>](#method-remove_translation_id) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-set_default_color" href="#method-set_default_color">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_default_color</span>](#method-set_default_color) ( `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-should_execute_this_branch" href="#method-should_execute_this_branch">**<span class="hljs-attribute">func</span> [<span class="hljs-title">should_execute_this_branch</span>](#method-should_execute_this_branch) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



to be overridden by sub-classes only called if can_contain_events is true and the previous event was an end-branch event return true if this event should be executed if the previous event was an end-branch event basically only important for the Condition event but who knows. Some day someone might need this.

---



<a class="header" id="method-to_text" href="#method-to_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">to_text</span>](#method-to_text) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



returns a readable presentation of the event (This is how it's stored) by default it uses a shortcode format, but can be overridden

---



<a class="header" id="method-update_text_version" href="#method-update_text_version">**<span class="hljs-attribute">func</span> [<span class="hljs-title">update_text_version</span>](#method-update_text_version) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Call this if you updated an event and want the changes to be saved.

---

