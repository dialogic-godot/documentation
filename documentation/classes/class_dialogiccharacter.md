
<div class="header-banner purple">
<div class="header-label purple">DialogicCharacter</div>
</div>

*This contains the source code documentation of the class `DialogicCharacter`.*
        
# DialogicCharacter
**Inherits:** Resource

Resource that represents a character in dialog. Manages/contains portraits, custom info and translation of characters.
## Properties
Name | Type | Default 
--- | --- | --- 
color | [Color](https://docs.godotengine.org/en/latest/classes/class_color.html#class-color) |  `Color(0, 0, 0, 1)` 
custom_info | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
default_portrait | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
description | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
display_name | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |  `""` 
mirror | [bool](https://docs.godotengine.org/en/latest/classes/class_bool.html#class-bool) |  `false` 
nicknames | [Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array) |   
offset | [Vector2](https://docs.godotengine.org/en/latest/classes/class_vector2.html#class-vector2) |  `Vector2(0, 0)` 
portraits | [Dictionary](https://docs.godotengine.org/en/latest/classes/class_dictionary.html#class-dictionary) |   
scale | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |  `1.0` 
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">add_translation_id</span>](#property-add_translation_id) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_character_name</span>](#property-get_character_name) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_display_name_translated</span>](#property-get_display_name_translated) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_nicknames_translated</span>](#property-get_nicknames_translated) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_portrait_info</span>](#property-get_portrait_info) ( `portrait_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_property_translation_key</span>](#property-get_property_translation_key) ( `property`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">get_set_translation_id</span>](#property-get_set_translation_id) ( ) 
<span class="hljs-attribute">void</span> | [<span class="hljs-title">remove_translation_id</span>](#property-remove_translation_id) ( ) 
--- 
## Constants


<a class="header" id="constant-NAME" href="#constant-NAME">**<span class="hljs-attribute">const</span> <span class="hljs-title">NAME</span><span class="hljs-comment"> = 0</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---


<a class="header" id="constant-NICKNAMES" href="#constant-NICKNAMES">**<span class="hljs-attribute">const</span> <span class="hljs-title">NICKNAMES</span><span class="hljs-comment"> = 1</span>**</a>



 <span style = "color: gray">*No description available.*</span> 

---
## Property Descriptions



<a class="header" id="property-add_translation_id" href="#property-add_translation_id">**<span class="hljs-attribute">void</span> [<span class="hljs-title">add_translation_id</span>](#property-add_translation_id) ( )** </a>



Adds a translation ID to the character.

---



<a class="header" id="property-get_character_name" href="#property-get_character_name">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_character_name</span>](#property-get_character_name) ( )** </a>



Returns the name of the file (without the extension).

---



<a class="header" id="property-get_display_name_translated" href="#property-get_display_name_translated">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_display_name_translated</span>](#property-get_display_name_translated) ( )** </a>



Translates and returns the display name of the character.

---



<a class="header" id="property-get_nicknames_translated" href="#property-get_nicknames_translated">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_nicknames_translated</span>](#property-get_nicknames_translated) ( )** </a>



Translates the nicknames of the characters and then returns them as an array of strings.

---



<a class="header" id="property-get_portrait_info" href="#property-get_portrait_info">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_portrait_info</span>](#property-get_portrait_info) ( `portrait_name`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) )** </a>



Returns the info of the given portrait. Uses the default portrait if the given portrait doesn't exist.

---



<a class="header" id="property-get_property_translation_key" href="#property-get_property_translation_key">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_property_translation_key</span>](#property-get_property_translation_key) ( `property`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )** </a>



Checks `property` and matches it to a translation key.  Undefined behaviour if an invalid integer is passed.

---



<a class="header" id="property-get_set_translation_id" href="#property-get_set_translation_id">**<span class="hljs-attribute">void</span> [<span class="hljs-title">get_set_translation_id</span>](#property-get_set_translation_id) ( )** </a>



Returns the character's translation ID. Adds a translation ID to the character if it doesn't have one.

---



<a class="header" id="property-remove_translation_id" href="#property-remove_translation_id">**<span class="hljs-attribute">void</span> [<span class="hljs-title">remove_translation_id</span>](#property-remove_translation_id) ( )** </a>



Removes the translation ID from the character.

---

