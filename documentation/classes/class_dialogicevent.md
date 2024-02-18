
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
can_contain_events | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
created_by_button | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
dialogic | [DialogicGameHandler](class_dialogicgamehandler.md) |  `null` 
dialogic_color_name | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
disable_editor_button | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
display_name | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
editor_list | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |   
empty_lines_above | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
end_branch_event | [DialogicEndBranchEvent](class_dialogicendbranchevent.md) |  `null` 
event_category | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"Other"` 
event_color | [Color](https://docs.godotengine.org/en/latest/classes/class_color.html#class-color) |  `Color(0.984314, 0.694118, 0.235294, 1)` 
event_name | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"Event"` 
event_node_as_text | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
event_node_ready | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
event_sorting_index | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
expand_by_default | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
help_page_path | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
needs_indentation | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
wants_to_group | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_body_edit</span>](#property-add_body_edit) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `editor_type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `14`, `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_body_line_break</span>](#property-add_body_line_break) ( `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_header_button</span>](#property-add_header_button) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `callable`: [Callable](https://docs.godotengine.org/en/latest/classes/class_callable.html#class-callable), `tooltip`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `icon`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_header_edit</span>](#property-add_header_edit) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `editor_type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `14`, `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_header_label</span>](#property-add_header_label) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_translation_id</span>](#property-add_translation_id) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">can_be_translated</span>](#property-can_be_translated) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">execute</span>](#property-execute) ( `_dialogic_game_handler`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">finish</span>](#property-finish) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">from_text</span>](#property-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_end_branch_control</span>](#property-get_end_branch_control) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_event_editor_info</span>](#property-get_event_editor_info) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_property_translated</span>](#property-get_property_translated) ( `property_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_property_translation_key</span>](#property-get_property_translation_key) ( `property_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_shortcode</span>](#property-get_shortcode) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">is_string_full_event</span>](#property-is_string_full_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">is_valid_event</span>](#property-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">parse_shortcode_parameters</span>](#property-parse_shortcode_parameters) ( `shortcode`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">remove_translation_id</span>](#property-remove_translation_id) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">set_default_color</span>](#property-set_default_color) ( `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">should_execute_this_branch</span>](#property-should_execute_this_branch) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">to_text</span>](#property-to_text) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">update_text_version</span>](#property-update_text_version) ( ) 
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


<a class="header" id="constant-CUSTOM" href="#constant-CUSTOM">**<span class="hljs-attribute">const</span> <span class="hljs-title">CUSTOM</span><span class="hljs-comment"> = 12</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-BUTTON" href="#constant-BUTTON">**<span class="hljs-attribute">const</span> <span class="hljs-title">BUTTON</span><span class="hljs-comment"> = 13</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-LABEL" href="#constant-LABEL">**<span class="hljs-attribute">const</span> <span class="hljs-title">LABEL</span><span class="hljs-comment"> = 14</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---

## Signals


<a class="header" id="signal-event_finished" href="#signal-event_finished">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">event_finished</span>](#signal-event_finished) ( `event_resource`: [DialogicEvent](class_dialogicevent.md) )** </a>



Emmited when the event finish. The signal is emmited with the event resource [code]event_resource[/code]

---



<a class="header" id="signal-event_started" href="#signal-event_started">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">event_started</span>](#signal-event_started) ( `event_resource`: [DialogicEvent](class_dialogicevent.md) )** </a>



Emmited when the event starts. The signal is emmited with the event resource [code]event_resource[/code]

---



<a class="header" id="signal-ui_update_needed" href="#signal-ui_update_needed">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">ui_update_needed</span>](#signal-ui_update_needed) ( )** </a>



Singal that notifies the visual editor block to update

---



<a class="header" id="signal-ui_update_warning" href="#signal-ui_update_warning">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">ui_update_warning</span>](#signal-ui_update_warning) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-add_body_edit" href="#property-add_body_edit">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_body_edit</span>](#property-add_body_edit) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `editor_type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `14`, `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-add_body_line_break" href="#property-add_body_line_break">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_body_line_break</span>](#property-add_body_line_break) ( `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-add_header_button" href="#property-add_header_button">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_header_button</span>](#property-add_header_button) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `callable`: [Callable](https://docs.godotengine.org/en/latest/classes/class_callable.html#class-callable), `tooltip`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `icon`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) = `null`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-add_header_edit" href="#property-add_header_edit">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_header_edit</span>](#property-add_header_edit) ( `variable`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `editor_type`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `14`, `extra_info`: [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) = `<unknown>`, `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-add_header_label" href="#property-add_header_label">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_header_label</span>](#property-add_header_label) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `condition`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-add_translation_id" href="#property-add_translation_id">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_translation_id</span>](#property-add_translation_id) ( )** </a>



This is automatically called, no need to use this.

---



<a class="header" id="property-build_event_editor" href="#property-build_event_editor">**<span class="hljs-attribute">void</span> [<span class="hljs-title">build_event_editor</span>](#property-build_event_editor) ( )** </a>



to be overwritten by the sub_classes

---



<a class="header" id="property-can_be_translated" href="#property-can_be_translated">**<span class="hljs-attribute">void</span> [<span class="hljs-title">can_be_translated</span>](#property-can_be_translated) ( )** </a>



Returns true if there is any translatable properties on this event. Overwrite [_get_translatable_properties()] to change this.

---



<a class="header" id="property-execute" href="#property-execute">**<span class="hljs-attribute">void</span> [<span class="hljs-title">execute</span>](#property-execute) ( `_dialogic_game_handler`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



Executes the event behaviour. In subclasses [_execute] (not this one) should be overriden!

---



<a class="header" id="property-finish" href="#property-finish">**<span class="hljs-attribute">void</span> [<span class="hljs-title">finish</span>](#property-finish) ( )** </a>



Ends the event behaviour.

---



<a class="header" id="property-from_text" href="#property-from_text">**<span class="hljs-attribute">void</span> [<span class="hljs-title">from_text</span>](#property-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



loads the variables from the string stored above by default it uses the shortcode format, but can be overridden

---



<a class="header" id="property-get_end_branch_control" href="#property-get_end_branch_control">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_end_branch_control</span>](#property-get_end_branch_control) ( )** </a>



to be overridden by sub-classes only called if can_contain_events is true. return a control node that should show on the END BRANCH node

---



<a class="header" id="property-get_event_editor_info" href="#property-get_event_editor_info">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_event_editor_info</span>](#property-get_event_editor_info) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_property_translated" href="#property-get_property_translated">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_property_translated</span>](#property-get_property_translated) ( `property_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



Call this whenever you are using a translatable property

---



<a class="header" id="property-get_property_translation_key" href="#property-get_property_translation_key">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_property_translation_key</span>](#property-get_property_translation_key) ( `property_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-get_shortcode" href="#property-get_shortcode">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_shortcode</span>](#property-get_shortcode) ( )** </a>



if this uses the short-code format, return the shortcode

---



<a class="header" id="property-get_shortcode_parameters" href="#property-get_shortcode_parameters">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_shortcode_parameters</span>](#property-get_shortcode_parameters) ( )** </a>



if this uses the short-code format, return the parameters and corresponding property names

---



<a class="header" id="property-is_string_full_event" href="#property-is_string_full_event">**<span class="hljs-attribute">void</span> [<span class="hljs-title">is_string_full_event</span>](#property-is_string_full_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



has to return true if this string seems to be a full event of this kind (only tested if is_valid_event() returned true) if a shortcode it used it will default to true if the string ends with ']'

---



<a class="header" id="property-is_valid_event" href="#property-is_valid_event">**<span class="hljs-attribute">void</span> [<span class="hljs-title">is_valid_event</span>](#property-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



has to return true, if the given string can be interpreted as this event by default it uses the shortcode formta, but can be overridden

---



<a class="header" id="property-parse_shortcode_parameters" href="#property-parse_shortcode_parameters">**<span class="hljs-attribute">void</span> [<span class="hljs-title">parse_shortcode_parameters</span>](#property-parse_shortcode_parameters) ( `shortcode`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



used to get all the shortcode parameters in a string as a dictionary

---



<a class="header" id="property-remove_translation_id" href="#property-remove_translation_id">**<span class="hljs-attribute">void</span> [<span class="hljs-title">remove_translation_id</span>](#property-remove_translation_id) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-set_default_color" href="#property-set_default_color">**<span class="hljs-attribute">void</span> [<span class="hljs-title">set_default_color</span>](#property-set_default_color) ( `value`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )** </a>



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-should_execute_this_branch" href="#property-should_execute_this_branch">**<span class="hljs-attribute">void</span> [<span class="hljs-title">should_execute_this_branch</span>](#property-should_execute_this_branch) ( )** </a>



to be overridden by sub-classes only called if can_contain_events is true and the previous event was an end-branch event return true if this event should be executed if the previous event was an end-branch event basically only important for the Condition event but who knows. Some day someone might need this.

---



<a class="header" id="property-to_text" href="#property-to_text">**<span class="hljs-attribute">void</span> [<span class="hljs-title">to_text</span>](#property-to_text) ( )** </a>



returns a readable presentation of the event (This is how it's stored) by default it uses a shortcode format, but can be overridden

---



<a class="header" id="property-update_text_version" href="#property-update_text_version">**<span class="hljs-attribute">void</span> [<span class="hljs-title">update_text_version</span>](#property-update_text_version) ( )** </a>



Call this if you updated an event and want the changes to be saved.

---

