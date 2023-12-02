# Dialogic 2 - 📚 Documentation

***This documentation is for the 2.x version of dialogic. This version is currently in alpha state so there will be breaking changes before the final release. So proceed with care!***

## What is dialogic?

The dialogic plugin allows to easily create in-game dialogs or visual novels with godot.

To do so it consists of multiple things:

1. An **event system** that is easy to extend (events are resources), and can load and save these events from a text format. It comes with over 20 events that can do most things you could want.

2. A **visual and text** editor built-in to godot to edit timelines that contain these events.

3. A collection of **ready-to-use custom nodes** that can display those events. You can use these to built your own designs or use one of the pre-made example scenes.

4. A **character system and editor** that allows to easily create characters with many portraits.

This only scratches the surface of what's possible though. Here is a small list of other things you can do:

- [Create events and timelines in code](/documentation/creating-timelines-in-code)

- Use built-in "text actions" like [speed], [pause], [signal], [portrait]

- Easy-to-use variables

- Create a glossary with strings that can be hovered to show information

- Translate dialogs in csv files

- Easily create custom events and display nodes

- Access most functionality from code e.g. `Dialogic.Portraits.change_portrait(Emilio, "happy")`, `Dialogic.Backgrounds.update_background("res://icon.png")`

## Getting started

You should follow [this introduction](/documentation/getting-started) if you want to get started with dialogic.

## Can I upgrade my current game made using Dialogic 1?

There are several things to overcome when upgrading from Dialogic 1. First of all, Dialogic 1 is exclusively for Godot 3, while Dialogic 2 is made for Godot 4. That means that you first need to make sure that your project works in Godot 4 by making the necessary adjustments required.

If you already made a lot of progress in your game, there is no reason to upgrade versions. We recommend you to stick to Godot 3 + Dialogic 1. But if you want to give it a go, thanks to @thebardsrc, there is a Dialogic 1 to Dialogic 2 converter available.
