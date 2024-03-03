
<div class="header-banner purple">
<div class="header-label purple">DialogicJumpEvent</div>
</div>

*This contains the source code documentation of the class `DialogicJumpEvent`.*
        
# DialogicJumpEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

# Settings
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">label_name</span>](#property-label_name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">timeline</span>](#property-timeline) | [DialogicTimeline](class_dialogictimeline.md) |   
[<span class="hljs-title">timeline_identifier</span>](#property-timeline_identifier) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_label_suggestions</span>](#method-get_label_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_timeline_suggestions</span>](#method-get_timeline_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">to_text</span>](#method-to_text) ( ) 
--- 
## Property Descriptions



<a class="header" id="property-label_name" href="#property-label_name">**<span class="hljs-attribute">var</span> <span class="hljs-title">label_name</span> <span style = "color: gray"> = </span> ""** 



If not empty, the event will try to find a Label event with this set as name. Empty by default..

---



<a class="header" id="property-timeline" href="#property-timeline">**<span class="hljs-attribute">var</span> <span class="hljs-title">timeline</span>** 



The timeline to jump to, if null then it's the current one. This setting should be a dialogic timeline resource.

---



<a class="header" id="property-timeline_identifier" href="#property-timeline_identifier">**<span class="hljs-attribute">var</span> <span class="hljs-title">timeline_identifier</span> <span style = "color: gray"> = </span> ""** 



Used to set the timeline resource from the unique name identifier and vice versa

---

## Method Descriptions



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-from_text" href="#method-from_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_label_suggestions" href="#method-get_label_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_label_suggestions</span>](#method-get_label_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_shortcode_parameters" href="#method-get_shortcode_parameters">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_shortcode_parameters</span>](#method-get_shortcode_parameters) ( )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-get_timeline_suggestions" href="#method-get_timeline_suggestions">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_timeline_suggestions</span>](#method-get_timeline_suggestions) ( `filter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `""` )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_valid_event" href="#method-is_valid_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-to_text" href="#method-to_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">to_text</span>](#method-to_text) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



############################################################################## SAVING/LOADING ##############################################################################

---

