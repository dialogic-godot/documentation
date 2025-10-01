
<div class="header-banner purple">
<div class="header-label purple">Settings</div>
</div>

*This contains the source code documentation of the class `subsystem_Settings`.*
        
# subsystem_Settings
**Inherits:** [DialogicSubsystem](class_dialogicsubsystem.md)

Subsystem that allows setting and getting settings that are automatically saved slot independent.
## Description
All settings that are stored in the project settings dialogic/settings section are supported. For example the text_speed setting is stored there. How to access this subsystem via code: ```gd Dialogic.Settings.text_speed = 0.05 ```  Settings stored there can also be changed with the Settings event.

## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">settings</span>](#property-settings) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |  `{}` 
--- 

## Methods
Returns | Method 
--- | --- 
<span style = "color: gray">void</span> | [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">get_setting</span>](#method-get_setting) ( `property`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
<span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span> | [<span class="hljs-title">has_setting</span>](#method-has_setting) ( `property`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset_all</span>](#method-reset_all) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">reset_setting</span>](#method-reset_setting) ( `property`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname) ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">connect_to_change</span>](#method-connect_to_change) ( `property`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname), `callable`: [Callable](https://docs.godotengine.org/en/latest/classes/class_callable.html#class-callable) ) 
--- 
## Property Descriptions



<a class="header" id="property-settings" href="#property-settings">**<span class="hljs-attribute">var</span> <span class="hljs-title">settings</span> <span style = "color: gray"> = </span> {}** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-clear_game_state" href="#method-clear_game_state">**<span class="hljs-attribute">func</span> [<span class="hljs-title">clear_game_state</span>](#method-clear_game_state) ( `_clear_flag`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) = `0` )</a>  ⇒ <span style = "color: gray">void</span>** 



Built-in, called by DialogicGameHandler.

---



<a class="header" id="method-get_setting" href="#method-get_setting">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_setting</span>](#method-get_setting) ( `property`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



Get a setting named `property`, if it does not exist, falls back to `default`.

---



<a class="header" id="method-has_setting" href="#method-has_setting">**<span class="hljs-attribute">func</span> [<span class="hljs-title">has_setting</span>](#method-has_setting) ( `property`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname) )</a>  ⇒ <span class="hljs-attribute">[bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool)</span>** 



Whether a setting has been set/stored before.

---



<a class="header" id="method-reset_all" href="#method-reset_all">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset_all</span>](#method-reset_all) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-reset_setting" href="#method-reset_setting">**<span class="hljs-attribute">func</span> [<span class="hljs-title">reset_setting</span>](#method-reset_setting) ( `property`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname) )</a>  ⇒ <span style = "color: gray">void</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-connect_to_change" href="#method-connect_to_change">**<span class="hljs-attribute">func</span> [<span class="hljs-title">connect_to_change</span>](#method-connect_to_change) ( `property`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname), `callable`: [Callable](https://docs.godotengine.org/en/latest/classes/class_callable.html#class-callable) )</a>  ⇒ <span style = "color: gray">void</span>** 



If a setting named `property` changes its value, this will emit `Callable`.

---

