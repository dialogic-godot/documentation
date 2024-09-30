
<div class="header-banner purple">
<div class="header-label purple">DialogicLayoutBase</div>
</div>

*This contains the source code documentation of the class `DialogicLayoutBase`.*
        
# DialogicLayoutBase
**Inherits:** [Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)

Base class that should be extended by custom layouts.
--- 

## Methods
Returns | Method 
--- | --- 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">add_layer</span>](#method-add_layer) ( `layer`: [DialogicLayoutLayer](class_dialogiclayoutlayer.md) ) 
<span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span> | [<span class="hljs-title">get_layer</span>](#method-get_layer) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) ) 
<span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span> | [<span class="hljs-title">get_layers</span>](#method-get_layers) ( ) 
<span style = "color: gray">void</span> | [<span class="hljs-title">apply_export_overrides</span>](#method-apply_export_overrides) ( ) 
<span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span> | [<span class="hljs-title">get_global_setting</span>](#method-get_global_setting) ( `setting`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) ) 
--- 
## Method Descriptions



<a class="header" id="method-add_layer" href="#method-add_layer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">add_layer</span>](#method-add_layer) ( `layer`: [DialogicLayoutLayer](class_dialogiclayoutlayer.md) )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



Method that adds a node as a layer

---



<a class="header" id="method-get_layer" href="#method-get_layer">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layer</span>](#method-get_layer) ( `index`: [int](https://docs.godotengine.org/en/latest/classes/class_int.html#class-int) )</a>  ⇒ <span class="hljs-attribute">[Node](https://docs.godotengine.org/en/latest/classes/class_node.html#class-node)</span>** 



Method that returns the given child

---



<a class="header" id="method-get_layers" href="#method-get_layers">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_layers</span>](#method-get_layers) ( )</a>  ⇒ <span class="hljs-attribute">[Array](https://docs.godotengine.org/en/latest/classes/class_array.html#class-array)</span>** 



Method to return all the layers

---



<a class="header" id="method-apply_export_overrides" href="#method-apply_export_overrides">**<span class="hljs-attribute">func</span> [<span class="hljs-title">apply_export_overrides</span>](#method-apply_export_overrides) ( )</a>  ⇒ <span style = "color: gray">void</span>** 



Method that is called to load the export overrides. This happens when the style is first introduced, but also when switching to a different style using the same scene!

---



<a class="header" id="method-get_global_setting" href="#method-get_global_setting">**<span class="hljs-attribute">func</span> [<span class="hljs-title">get_global_setting</span>](#method-get_global_setting) ( `setting`: [StringName](https://docs.godotengine.org/en/latest/classes/class_stringname.html#class-stringname), `default`: [Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant) )</a>  ⇒ <span class="hljs-attribute">[Variant](https://docs.godotengine.org/en/latest/classes/class_variant.html#class-variant)</span>** 



Returns a setting on this base. This is useful so that layers can share settings like base_color, etc.

---

