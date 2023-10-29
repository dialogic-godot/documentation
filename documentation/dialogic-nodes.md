---
title: Dialogic Nodes
---

![header_dialogic_nodes_layouts](/media/headers/dialogic_nodes_layouts.png)

To make timelines work in your your game, there have to be **Dialogic Nodes** in the tree. Usually this means dialogic will add a **layout scene** made out of DialogicNodes. This is what happens if you call Dialogic.start() and can be set in the [Style editor](/documentation/styles-and-layouts). It is also possible to integrate DialogicNodes into your existing UI. 

## What is a dialogic node?

Many events have nodes that you need if you want them to actually affect the game: 

- **Text event:** DialogText, NameLabel, NextIndicator, TypingSound

- **Character event:** PortraitContainer

- **Choice event:** ChoiceButton, ChoiceSound

- **Background event:** Background

- **Text Input event:** TextInput

Here are some things to know about dialogic nodes:

- Dialogic Nodes provide very different functionality. Because of that, they have very different properties. Learn more about each Dialogic Node by adding it to your scene and taking a look at the inspector.

- Some Dialogic Nodes use settings from the dialogic settings page. 
  A general rule-of-thumbs is that settings that should be the same for all instances of a dialogic node are usually a dialogic setting, while things that might change from node to node, are a property.

## Using dialogic nodes

You can add these nodes with the usual `Add Node` window.

It's not important where they are placed in the tree, as they will be recognized by a group they are automatically added to.

Some dialogic nodes require a somewhat special setup. For example the TypingSound node expects to be the child of a DialogText node.

## Examples

You can take a look at the preset layout scenes in `addons/dialogic/Modules/DefaultLayouts`. 
