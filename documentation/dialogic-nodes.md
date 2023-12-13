<div class="header-banner tropical">
     <div class="header-label tropical">Dialogic Nodes</div>

</div>

*Dialogic Nodes are custom nodes provided by dialogic that handle the presentation of your timelines in your game.*

#### 📜 Content

- [1. Introduction](#1-introduction)
- [2. What is a dialogic node?](#2-what-is-a-dialogic-node)
- [3. Using dialogic nodes](#3-using-dialogic-nodes)

## 1. Introduction

Usually this means dialogic will add a **layout scene** made out of DialogicNodes. This is what happens if you call Dialogic.start() and can be set in the [Style editor](styles-and-layouts.md). It is also possible to integrate DialogicNodes into your existing UI.

This topic is closely related to [Styles and Layouts](styles-and-layouts.md), so take a look at that page if you haven't done so yet.

---

## 2. What is a dialogic node?

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

---

## 3. Using dialogic nodes

You can add these nodes with the usual `Add Node` window.

It's not important where they are placed in the tree, as they will be recognized by a group they are automatically added to.

Some dialogic nodes require a somewhat special setup. For example the TypingSound node expects to be the child of a DialogText node.
