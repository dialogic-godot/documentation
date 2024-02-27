
<div class="header-banner purple">
<div class="header-label purple">DialogicBackgroundTransition</div>
</div>

*This contains the source code documentation of the class `DialogicBackgroundTransition`.*
        
# DialogicBackgroundTransition
**Inherits:** [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)


## Properties
Name | Type | Default 
--- | --- | --- 
[<span class="hljs-title">bg_holder</span>](#property-bg_holder) | [DialogicNode_BackgroundHolder](class_dialogicnode_backgroundholder.md) |   
[<span class="hljs-title">next_scene</span>](#property-next_scene) | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |   
[<span class="hljs-title">next_texture</span>](#property-next_texture) | [ViewportTexture](https://docs.godotengine.org/en/latest/classes/class_viewporttexture.html#class-viewporttexture) |   
[<span class="hljs-title">prev_scene</span>](#property-prev_scene) | [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node) |   
[<span class="hljs-title">prev_texture</span>](#property-prev_texture) | [ViewportTexture](https://docs.godotengine.org/en/latest/classes/class_viewporttexture.html#class-viewporttexture) |   
[<span class="hljs-title">this_folder</span>](#property-this_folder) | [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) |   
[<span class="hljs-title">time</span>](#property-time) | [float](https://docs.godotengine.org/en/latest/classes/class_float.html#class-float) |   
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[ShaderMaterial](https://docs.godotengine.org/en/latest/classes/class_shadermaterial.html#class-shadermaterial)</span> | [<span class="hljs-title">set_shader</span>](#property-set_shader) ( `path_to_shader`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `<unknown>` ) 
<span class="hljs-attribute">[PropertyTweener](https://docs.godotengine.org/en/latest/classes/class_propertytweener.html#class-propertytweener)</span> | [<span class="hljs-title">tween_shader_progress</span>](#property-tween_shader_progress) ( `progress_parameter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `"progress"` ) 
--- 

## Signals


<a class="header" id="signal-transition_finished" href="#signal-transition_finished">**<span class="hljs-attribute">signal</span> [<span class="hljs-title">transition_finished</span>](#signal-transition_finished) ( )** </a>



 <span style = "color: gray">*No description available.*</span> 

---

## Property Descriptions



<a class="header" id="property-bg_holder" href="#property-bg_holder">**<span class="hljs-attribute">var</span> <span class="hljs-title">bg_holder</span>** 



Set before _fade() is called, will be the background holder (TextureRect)

---



<a class="header" id="property-next_scene" href="#property-next_scene">**<span class="hljs-attribute">var</span> <span class="hljs-title">next_scene</span>** 



Set before _fade() is called, will be the root node of the upcoming bg scene.

---



<a class="header" id="property-next_texture" href="#property-next_texture">**<span class="hljs-attribute">var</span> <span class="hljs-title">next_texture</span>** 



Set before _fade() is called, will be the viewport texture of the upcoming bg scene.

---



<a class="header" id="property-prev_scene" href="#property-prev_scene">**<span class="hljs-attribute">var</span> <span class="hljs-title">prev_scene</span>** 



Set before _fade() is called, will be the root node of the previous bg scene.

---



<a class="header" id="property-prev_texture" href="#property-prev_texture">**<span class="hljs-attribute">var</span> <span class="hljs-title">prev_texture</span>** 



Set before _fade() is called, will be the viewport texture of the previous bg scene.

---



<a class="header" id="property-this_folder" href="#property-this_folder">**<span class="hljs-attribute">var</span> <span class="hljs-title">this_folder</span> <span style = "color: gray"> = </span> <unknown>** 



Helper

---



<a class="header" id="property-time" href="#property-time">**<span class="hljs-attribute">var</span> <span class="hljs-title">time</span>** 



Set before _fade() is called, will be the requested time for the fade

---

## Methods Descriptions



<a class="header" id="method-set_shader" href="#method-set_shader">**<span class="hljs-attribute">func</span> [<span class="hljs-title">set_shader</span>](#property-set_shader) ( `path_to_shader`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `<unknown>` )</a>  ⇒ <span class="hljs-attribute">[ShaderMaterial](https://docs.godotengine.org/en/latest/classes/class_shadermaterial.html#class-shadermaterial)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---



<a class="header" id="method-tween_shader_progress" href="#method-tween_shader_progress">**<span class="hljs-attribute">func</span> [<span class="hljs-title">tween_shader_progress</span>](#property-tween_shader_progress) ( `progress_parameter`: [String](https://docs.godotengine.org/en/latest/classes/class_string.html#class-string) = `"progress"` )</a>  ⇒ <span class="hljs-attribute">[PropertyTweener](https://docs.godotengine.org/en/latest/classes/class_propertytweener.html#class-propertytweener)</span>** 



 <span style = "color: gray">*No description available.*</span> 

---

