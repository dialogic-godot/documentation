
<div class="header-banner purple">
<div class="header-label purple">DialogicAutoSkip</div>
</div>

*This contains the source code documentation of the class `DialogicAutoSkip`.*
        
# DialogicAutoSkip
**Inherits:** [RefCounted](https://docs.godotengine.org/en/latest/classes/class_refcounted.html#class-refcounted)

This class holds the settings for the Auto-Skip feature. Changing the variables will alter the behaviour of Auto-Skip.
## Description
Auto-Skip must be implemented per event.

## Properties
Name | Type | Default 
--- | --- | --- 
disable_on_unread_text | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
disable_on_user_input | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
enable_on_seen | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
enabled | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
skip_voice | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `true` 
time_per_event | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `0.1` 

## Signals


<a class="header" id="signal-toggled" href="#signal-toggled">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">toggled</span>](#signal-toggled) ( `is_enabled`: [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) )** </a>



Emitted whenever the Auto-Skip state changes, from `true` to `false` or vice-versa.

---

