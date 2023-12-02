# Custom Portraits

![header_custom_portraits](/media/headers/custom_portraits.png)


## 📜 Content

- [1. Introduction](#1-introduction)
- [2. Requirements](#2-requirements)
- [3. Overwriting methods](#3-overwriting-methods)
- [4. Export Overrides](#4-export-overrides)
- [5. Examples](#5-examples)

## 1. Introduction

Oftentimes you want something more complex than a simple image: an animated image (e.g. AnimatedSprite), a rigged and animated character, a character with a single body but many face-variations or something else entirely.

To achieve these, you will have to create a **custom portrait scene**.

One scene can be used for one or multiple portraits. If a scene is used for multiple portraits, then switching between them will not re-instance the scene and only call `_update_portrait(@portrait_name)` on that scene (see more below). This allows you to even animate from one portrait to the next.

## 2. Requirements

There are not a lot of requirements for portrait scenes:

- **Root needs to be Node2D or Control:**
  *The root nodes needs a position and scale property, so it must be a Node2D or Control node (or a sub-class).
  Because the root will act as the "pivot-point" it's suggested to use a simple node like Marker2D and have all functional nodes (like sprites, animation players etc.) be children of it.*
- **Root script extends DialogicPortrait:**
  *The root nodes script should extend the DialogicPortrait class and overwrite some of it's methods.*

## 3. Overwriting methods

You can customize the behaviour by adding a script to the root node and adding specific methods to it. Like `_ready` or `_process` these will be called automatically by dialogic when needed and if implemented:

- **_update_portrait(@character, @portrait_name):**
  *This method is called when the portrait is instanced and when a change to another portrait using the same scene is performed. For example you could play a specific animation in an AnimatedSprite based on the portrait name or show a specific image.*

- **_set_mirror(@mirrored):**
  *Different scenes might want to mirror differently (AnimationSprite.flip_h; self.scale.x = -1, etc.). Thus, you will have to implement this functionality yourself.*

- **_get_covered_rect() -> Rect2:**
  *This is used for correctly sizing your scene, as it's pretty much impossible to know the size of your portrait. If you implement this and return a rect2 that covers your portrait (relative to the root nodes position), the portrait_containers size modes and the character editors `Full View` will work.*

- **_set_extra_data(@data_string):**
  *The Character event Join/Update mode allow to specify some extra information in the text editor. If some information is given, this method will be called. This can be very useful to enable certain things. For example your character could have different modes or items.*

- **_should_do_portrait_update(@character, @portrait_name):**
  *Rarely needed, but if overridden this will be checked, if the portrait change is performed to a portrait with the same scene. If you return false, then this instance will be deleted and a new instance will be made. If not implemented this defaults to true, meaning this instance will be used for the portrait update too.*

## 4. Export overrides

If you add exported variables to your scenes script, you can change their values in the portrait settings in the character editor.
This allows you to change these values for different portraits that use the same scene.

```gdscript
@export_file var image := ""
@export var modulation := Color.WHITE
```

*Would add a Image and Modulation settings to all portraits using this scene.*

## 5. Examples

Besides the DefaultPortrait scene (in addons/dialogic/Other) there are some example scenes in `addons/dialogic/Example Assets/Portraits`, that implement some or all of these methods to achieve different effects.

Take a look at them if you feel unsure how to implement a valid portrait scene!
