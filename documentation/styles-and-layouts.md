<div class="header-banner dawn">
     <div class="header-label dawn">Styles & Layouts</div>
</div>

*This page is all about how dialogic can display timelines in your game using Styles, Layouts and Dialogic Nodes.*

## 📜 Content
[toc]

## 1. Introduction

One important aspect of Dialogic is how it allows you to display your timelines. To achieve this, there are a number of systems working together: Dialogic Nodes, Layout Scenes and Styles.

**Dialogic Nodes** are nodes that can be placed in any scene. These nodes will be activated by dialogic and do wildly different things, from displaying text, labels or choices to playing sounds or defining a clickable area.

**Layout Scenes** are scenes that contain both Dialogic Nodes, other Godot Control nodes, and custom scripts and provide a standalone UI-part. For example, there is a `VisualNovel Textbox Scene`, a `Glossary Popup Scene` or a `Centered Choices Scene`.

**Dialogic Styles** are a resource that holds a combination of layout scenes and allows for setting them. This is the easiest way to modify the look of Dialogic, as styles can be edited in Dialogic's Style Editor.

## 2. Working with styles

You can find a video walkthrough of Dialogic styles here: [Dialogic 2 - New Style System - YouTube](https://www.youtube.com/watch?v=TLnzSzqBwu4)

A style is made up of:

- One `Base` layout scene (of type `DialogicLayoutBase`) and settings for that scene.

- A list of `Layer` layout scenes (of type `DialogicLayoutLayer`) and settings for each layer.

In the style editor, you can

- Add new styles (either starting empty or from a premade style)

- Rename Styles

Add, replace, or remove layers (both premade scenes and custom scenes)

- Set all kinds of settings on any of the scenes that are part of that style

- Make one of the premade layers or a whole style custom

- Make an inherited style from another style (inherits scenes and default settings)

- Change the default style

### 2.1 Using styles in game

You can switch between different styles with the `Change Style` event, by calling `Dialogic.Styles.load_style()` before calling `Dialogic.start()`, or by assigning a style to a character.

## 3. Custom Styles & Layouts

You can customize all parts of this "Displaying" part of Dialogic.

### 3.1 Custom styles

The simplest is creating a custom style by combining different layers and changing their settings.

### 3.2 Custom Layout Scenes

The next step would be to customize part of your layout (one of the scenes) beyond what's possible with the provided settings.

An easy way to do this is to use the "Make Custom" button above the layer list and select "Current Layer". 
This will create a copy of that layer's scene, which you can edit in Godot. This is what you would do if you generally like, e.g., the text box, but would like to change something about it that's impossible with just the settings.

> [!TIP]
> When editing a layout that's been made custom, be careful which sub-resources (e.g. scripts, fonts, images, etc.) might still be inside the addons/dialogic folder.
> If you modify these the changes might be lost when updating dialogic.
> I recommend making any sub-resource "unique" before modifying it.
> Some, like the scenes root-script however are usually made custom automatically when using "Make Custom".

Alternatively, you can start a custom layout scene from scratch.

- Your scene's root node has to have a script that extends from either `DialogicLayoutBase` or `DialogicLayoutLayer` depending on your use-case.

- In your scene root script, you can export variables, which will appear as settings in Dialogic's style editor. Grouping them with @export_group and @export_subgroup makes it even nicer. Note that not all types are supported here.

- If you want to utilize Dialogic's style system, then you should apply any @exported settings in a method called `_apply_export_overrides()` which is called whenever the style changes.

You can add your custom scene effortlessly by either using `Add Layer` or `Replace Layer` above the layer list.

### 3.3 Custom nodes

While Dialogic's modules usually expect the nodes that display them to be made in a certain way, that doesn't prevent you from actually customizing the nodes themselves. Each dialogic node is just a normal control node with a script attached to it. Usually, dialogic nodes interact with dialogic subsystems through a group they add themselves to.

Note that in most cases, reacting to some Dialogic signals (or signals of existing dialogic nodes) can be way easier than creating a custom version of a dialogic node.
