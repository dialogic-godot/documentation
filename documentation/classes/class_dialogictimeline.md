
<div class="header-banner purple">
<div class="header-label purple">DialogicTimeline</div>
</div>

*This contains the source code documentation of the class `DialogicTimeline`.*
        
# DialogicTimeline
**Inherits:** [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource)

Resource that defines a list of events. It can store them as text and load them from text too.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">events</span>](#property-events) | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |  `[]` 
[<span class="hljs-title">events_processed</span>](#property-events_processed) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">text_lines_indexed</span>](#property-text_lines_indexed) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{}` 
[<span class="hljs-title">indent_format</span>](#property-indent_format) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `"\t"` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">get_event</span>](#method-get_event) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#method-from_text) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">as_text</span>](#method-as_text) ( ) 
<span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span> | [<span class="hljs-title">get_index_from_text_line</span>](#method-get_index_from_text_line) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `line`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">process</span>](#method-process) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">clean</span>](#method-clean) ( ) 
<span class="hljs-attribute">[DialogicEvent](class_dialogicevent.md)</span> | [<span class="hljs-title">event_from_string</span>](#method-event_from_string) ( `event_content`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `event_cache`: [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) ) 
--- 
## Property Descriptions



<a class="header" id="property-events" href="#property-events">**<span class="hljs-attribute">var</span> <span class="hljs-title">events</span> <span style = "color: gray"> = </span> []** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-events_processed" href="#property-events_processed">**<span class="hljs-attribute">var</span> <span class="hljs-title">events_processed</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-text_lines_indexed" href="#property-text_lines_indexed">**<span class="hljs-attribute">var</span> <span class="hljs-title">text_lines_indexed</span> <span style = "color: gray"> = </span> {}** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-indent_format" href="#property-indent_format">**<span class="hljs-attribute">var</span> <span class="hljs-title">indent_format</span> <span style = "color: gray"> = </span> "\t"** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-get_event" href="#method-get_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_event</span>](#method-get_event) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



Helper method

---



<a class="header" id="method-from_text" href="#method-from_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">from_text</span>](#method-from_text) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



Parses the lines as seperate events and insert them in an array, so they can be converted to DialogicEvent's when processed later

---



<a class="header" id="method-as_text" href="#method-as_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">as_text</span>](#method-as_text) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Stores all events in their text format and returns them as a string

---



<a class="header" id="method-get_index_from_text_line" href="#method-get_index_from_text_line">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_index_from_text_line</span>](#method-get_index_from_text_line) ( `text`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `line`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int)</span>** 



Returns the index of the event that corresponds to a specific line

---



<a class="header" id="method-process" href="#method-process">**<span class="hljs-attribute">func</span> [<span class="hljs-title">process</span>](#method-process) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Method that loads all the event resources from the strings, if it wasn't done before

---



<a class="header" id="method-clean" href="#method-clean">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clean</span>](#method-clean) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



This method makes sure that all events in a timeline are correctly reset

---



<a class="header" id="method-event_from_string" href="#method-event_from_string">**<span class="hljs-attribute">func</span> [<span class="hljs-title">event_from_string</span>](#method-event_from_string) ( `event_content`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string), `event_cache`: [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) )</a>  ⇒ <span class="hljs-attribute">[DialogicEvent](class_dialogicevent.md)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

