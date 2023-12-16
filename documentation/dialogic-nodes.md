<div class="header-banner tropical">
     <div class="header-label tropical">Dialogic Nodes</div>

</div>

*Dialogic Nodes are custom nodes provided by Dialogic that handle the presentation of your timelines in your game.*

## 📜 Content
[toc]

## 1. Introduction

Usually, this means Dialogic will add a **layout scene** made of `DialogicNodes`. This is what happens if you call `Dialogic.start()` and can be set in the [Style editor](styles-and-layouts.md). It is also possible to integrate `DialogicNodes` into your existing UI.

This topic is closely related to [Styles and Layouts](styles-and-layouts.md), so take a look at that page if you haven't done so yet.

---

## 2. What is a dialogic node?

Many events have nodes that you need if you want them to actually affect the game:

- **Text event:** `DialogText`, `NameLabel`, `NextIndicator`, `TypingSound`

- **Character event:** `PortraitContainer`

- **Choice event:** `ChoiceButton`, `ChoiceSound`

- **Background event:** Background

- **Text Input event:** `TextInput`

Here are some things to know about dialogic nodes:

- Dialogic Nodes provide very different functionality. Hence, they have very different properties. Learn more about each Dialogic Node by adding it to your scene and taking a look at the inspector.

- Some Dialogic Nodes use settings from the dialogic settings page.
  A general rule-of-thumb is that settings that should be the same for all instances of a Dialogic node are usually a Dialogic setting, while things that might change from node to node are properties.

---

## 3. Using dialogic nodes

You can add these nodes with the usual `Add Node` window.

It's not relevant where they are placed in the tree, as they will be recognized by the group they are automatically added to.

Some dialogic nodes require a somewhat special setup. For example, the `TypingSound` node expects to be the child of a `DialogText` node.
