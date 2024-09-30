
<div class="header-banner purple">
<div class="header-label purple">DialogicConditionEvent</div>
</div>

*This contains the source code documentation of the class `DialogicConditionEvent`.*
        
# DialogicConditionEvent
**Inherits:** [DialogicEvent](class_dialogicevent.md)

Event that allows branching a timeline based on a condition.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">condition_type</span>](#property-condition_type) | [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) |  `0` 
[<span class="hljs-title">condition</span>](#property-condition) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">should_execute_this_branch</span>](#method-should_execute_this_branch) ( ) 
<span class="hljs-attribute">[Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)</span> | [<span class="hljs-title">get_end_branch_control</span>](#method-get_end_branch_control) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">to_text</span>](#method-to_text) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( ) 
--- 
## Constants


<a class="header" id="constant-IF" href="#constant-IF">**<span class="hljs-attribute">const</span> <span class="hljs-title">IF</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ELIF" href="#constant-ELIF">**<span class="hljs-attribute">const</span> <span class="hljs-title">ELIF</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ELSE" href="#constant-ELSE">**<span class="hljs-attribute">const</span> <span class="hljs-title">ELSE</span><span class="hljs-comment"> = 2</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-condition_type" href="#property-condition_type">**<span class="hljs-attribute">var</span> <span class="hljs-title">condition_type</span> <span style = "color: gray"> = </span> 0** 



# Settings condition type (see ). Defaults to if.

---



<a class="header" id="property-condition" href="#property-condition">**<span class="hljs-attribute">var</span> <span class="hljs-title">condition</span> <span style = "color: gray"> = </span> ""** 



The condition as a string. Will be executed as an Expression.

---

## Method Descriptions



<a class="header" id="method-should_execute_this_branch" href="#method-should_execute_this_branch">**<span class="hljs-attribute">func</span> [<span class="hljs-title">should_execute_this_branch</span>](#method-should_execute_this_branch) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



only called if the previous event was an end-branch event return true if this event should be executed if the previous event was an end-branch event

---



<a class="header" id="method-get_end_branch_control" href="#method-get_end_branch_control">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_end_branch_control</span>](#method-get_end_branch_control) ( )</a>  ⇒ <span class="hljs-attribute">[Control](https://docs.godotengine.org/en/latest/classes/class_control.html#class-control)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-to_text" href="#method-to_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">to_text</span>](#method-to_text) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-from_text" href="#method-from_text">**<span class="hljs-attribute">func</span> [<span class="hljs-title">from_text</span>](#method-from_text) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-is_valid_event" href="#method-is_valid_event">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_valid_event</span>](#method-is_valid_event) ( `string`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-build_event_editor" href="#method-build_event_editor">**<span class="hljs-attribute">func</span> [<span class="hljs-title">build_event_editor</span>](#method-build_event_editor) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

