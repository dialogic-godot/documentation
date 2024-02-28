
<div class="header-banner purple">
<div class="header-label purple">DialogicCharacter</div>
</div>

*This contains the source code documentation of the class `DialogicCharacter`.*
        
# DialogicCharacter
**Inherits:** [Resource](https://docs.godotengine.org/en/latest/classes/class_resource.html#class-resource)

Resource that represents a character in dialog. Manages/contains portraits, custom info and translation of characters.
## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">color</span>](#property-color) | [Color](https://docs.godotengine.org/en/latest/classes/class_color.html#class-color) |  `Color(0, 0, 0, 1)` 
[<span class="hljs-title">custom_info</span>](#property-custom_info) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">default_portrait</span>](#property-default_portrait) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">description</span>](#property-description) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">display_name</span>](#property-display_name) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
[<span class="hljs-title">mirror</span>](#property-mirror) | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
[<span class="hljs-title">nicknames</span>](#property-nicknames) | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |   
[<span class="hljs-title">offset</span>](#property-offset) | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |  `Vector2(0, 0)` 
[<span class="hljs-title">portraits</span>](#property-portraits) | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
[<span class="hljs-title">scale</span>](#property-scale) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `1.0` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">add_translation_id</span>](#property-add_translation_id) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_character_name</span>](#property-get_character_name) ( ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_display_name_translated</span>](#property-get_display_name_translated) ( ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_nicknames_translated</span>](#property-get_nicknames_translated) ( ) 
<span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span> | [<span class="hljs-title">get_portrait_info</span>](#property-get_portrait_info) ( `portrait_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_property_translation_key</span>](#property-get_property_translation_key) ( `property`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span> | [<span class="hljs-title">get_set_translation_id</span>](#property-get_set_translation_id) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">remove_translation_id</span>](#property-remove_translation_id) ( ) 
--- 
## Constants


<a class="header" id="constant-NAME" href="#constant-NAME">**<span class="hljs-attribute">const</span> <span class="hljs-title">NAME</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-NICKNAMES" href="#constant-NICKNAMES">**<span class="hljs-attribute">const</span> <span class="hljs-title">NICKNAMES</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-color" href="#property-color">**<span class="hljs-attribute">var</span> <span class="hljs-title">color</span> <span style = "color: gray"> = </span> Color(0, 0, 0, 1)** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-custom_info" href="#property-custom_info">**<span class="hljs-attribute">var</span> <span class="hljs-title">custom_info</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-default_portrait" href="#property-default_portrait">**<span class="hljs-attribute">var</span> <span class="hljs-title">default_portrait</span> <span style = "color: gray"> = </span> ""** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-description" href="#property-description">**<span class="hljs-attribute">var</span> <span class="hljs-title">description</span> <span style = "color: gray"> = </span> ""** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-display_name" href="#property-display_name">**<span class="hljs-attribute">var</span> <span class="hljs-title">display_name</span> <span style = "color: gray"> = </span> ""** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-mirror" href="#property-mirror">**<span class="hljs-attribute">var</span> <span class="hljs-title">mirror</span> <span style = "color: gray"> = </span> false** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-nicknames" href="#property-nicknames">**<span class="hljs-attribute">var</span> <span class="hljs-title">nicknames</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-offset" href="#property-offset">**<span class="hljs-attribute">var</span> <span class="hljs-title">offset</span> <span style = "color: gray"> = </span> Vector2(0, 0)** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-portraits" href="#property-portraits">**<span class="hljs-attribute">var</span> <span class="hljs-title">portraits</span> <span style = "color: gray"> = </span> <unknown>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="property-scale" href="#property-scale">**<span class="hljs-attribute">var</span> <span class="hljs-title">scale</span> <span style = "color: gray"> = </span> 1.0** 



 <span style = "color: gray">*No description available.*</span> 

---

## Method Descriptions



<a class="header" id="method-add_translation_id" href="#method-add_translation_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_translation_id</span>](#property-add_translation_id) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Adds a translation ID to the character.

---



<a class="header" id="method-get_character_name" href="#method-get_character_name">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_character_name</span>](#property-get_character_name) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the name of the file (without the extension).

---



<a class="header" id="method-get_display_name_translated" href="#method-get_display_name_translated">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_display_name_translated</span>](#property-get_display_name_translated) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Translates and returns the display name of the character.

---



<a class="header" id="method-get_nicknames_translated" href="#method-get_nicknames_translated">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_nicknames_translated</span>](#property-get_nicknames_translated) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



Translates the nicknames of the characters and then returns them as an array of strings.

---



<a class="header" id="method-get_portrait_info" href="#method-get_portrait_info">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_portrait_info</span>](#property-get_portrait_info) ( `portrait_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )</a>  ⇒ <span class="hljs-attribute">[Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary)</span>** 



Returns the info of the given portrait. Uses the default portrait if the given portrait doesn't exist.

---



<a class="header" id="method-get_property_translation_key" href="#method-get_property_translation_key">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_property_translation_key</span>](#property-get_property_translation_key) ( `property`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Checks `property` and matches it to a translation key.  Undefined behaviour if an invalid integer is passed.

---



<a class="header" id="method-get_set_translation_id" href="#method-get_set_translation_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_set_translation_id</span>](#property-get_set_translation_id) ( )</a>  ⇒ <span class="hljs-attribute">[String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string)</span>** 



Returns the character's translation ID. Adds a translation ID to the character if it doesn't have one.

---



<a class="header" id="method-remove_translation_id" href="#method-remove_translation_id">**<span class="hljs-attribute">func</span> [<span class="hljs-title">remove_translation_id</span>](#property-remove_translation_id) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Removes the translation ID from the character.

---

