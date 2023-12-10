
# Introduction to Dialogic 2

```admonish info
This documentation is for Dialogic 2. 

Dialogic 2 is still in-development and marked as Alpha, there may be workflow breakage!
```

## What is Dialogic 2?

The Dialogic plugin allows you to easily create in-game dialogs or fully fledged **Visual Novels** with Godot. 

Dialogic 2 empowers you with:

1. **Timelines**! They control the flow of your story. They can be edited in a writer-friendly **Visual Editor** or your editor of choice.
   
2. **Events**! Each timeline contains events, and Dialogic equips you with many built-ones to get your story started today!

3. **Customization!** Cannot find the right Event? Find out what others created, or create your own specific Events with very little code. They flow right into the Visual Editor too!

4. **Character system and editor** that allows you to easily create characters with the images you desire ("portraits").

This is just scratching the surface of what's possible. 
Here is a small list of other things you can do:


- [Create events and timelines in code](/documentation/creating-timelines-in-code)

- Use built-in "text actions" like `[speed]`, `[pause]`, `[signal]`, `[portrait]`

- Easy-to-use variables in your timelines!

- Create a glossary with strings that can be hovered over to show information.

- Translate characters and timelines with the integrated CSV file system!

- Easily create custom events; they are all resources.

- Access functionality from code, for instance, "Dialogic.Portraits.change_portrait(Emilio, "happy")`, `Dialogic.Backgrounds.update_background("res://icon.png")`

## How do I get started?

First, [let's get Dialogic up and running](getting-started)! After this step, the numerous pages on the left-side navigation bar will aid you with your dialog-driven game adventure! 

Cannot find the right page? Try the search or open an issue on the GitHub repository!

## Can I upgrade my current game made using Dialogic 1?

There are several things to overcome when upgrading from Dialogic 1. First, Dialogic 1 is exclusively for Godot 3, while Dialogic 2 is made for Godot 4. That means that you first need to make sure that your project works in Godot 4 by making the necessary adjustments.

If you have already made a lot of progress in your game, there is no reason to upgrade. We recommend you stick to Godot 3 and Dialogic 1. But if you want to give it a try, thanks to our contributors, there is a Dialogic 1 to Dialogic 2 converter available.
