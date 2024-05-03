
<div class="header-banner purple">
<div class="header-label purple">DialogicManualAdvance</div>
</div>

*This contains the source code documentation of the class `DialogicManualAdvance`.*
        
# DialogicManualAdvance
**Inherits:** [RefCounted](https://docs.godotengine.org/en/latest/classes/class_refcounted.html#class-refcounted)

This class holds the settings for the Manual-Advance feature. Changing the variables will alter the behaviour of manually advancing the timeline, e.g. using the input action.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">disabled_until_next_event</span>](#property-disabled_until_next_event) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">system_enabled</span>](#property-system_enabled) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">is_enabled</span>](#method-is_enabled) ( ) 
--- 
## Constants


<a class="header" id="constant-STATE_INFO_KEY" href="#constant-STATE_INFO_KEY">**<span class="hljs-attribute">const</span> <span class="hljs-title">STATE_INFO_KEY</span><span class="hljs-comment"> = "manual_advance"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-ENABLED_STATE_KEY" href="#constant-ENABLED_STATE_KEY">**<span class="hljs-attribute">const</span> <span class="hljs-title">ENABLED_STATE_KEY</span><span class="hljs-comment"> = "enabled"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-DISABLED_UNTIL_NEXT_EVENT_STATE_KEY" href="#constant-DISABLED_UNTIL_NEXT_EVENT_STATE_KEY">**<span class="hljs-attribute">const</span> <span class="hljs-title">DISABLED_UNTIL_NEXT_EVENT_STATE_KEY</span><span class="hljs-comment"> = "temp_disabled"</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-disabled_until_next_event" href="#property-disabled_until_next_event">**<span class="hljs-attribute">var</span> <span class="hljs-title">disabled_until_next_event</span> <span style = "color: gray"> = </span> false** 



If `true`, Manual-Advance will be deactivated until the next event.  Use this flag to create a temporary Manual-Advance block.  Overrides `system_enabled` when true.

---



<a class="header" id="property-system_enabled" href="#property-system_enabled">**<span class="hljs-attribute">var</span> <span class="hljs-title">system_enabled</span> <span style = "color: gray"> = </span> true** 



If `true`, Manual-Advance will stay enabled until this is set to `false`.  Use this flag to activate or disable Manual-Advance mode.  Can be temporarily overwritten by `disabled_until_next_event`.

---

## Method Descriptions



<a class="header" id="method-is_enabled" href="#method-is_enabled">**<span class="hljs-attribute">func</span> [<span class="hljs-title">is_enabled</span>](#method-is_enabled) ( )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Whether the player can use Manual-Advance to advance the timeline.

---

