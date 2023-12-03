![header_getting_started](/media/headers/getting_started.png)

## 📜 Content

- [1. Installation & Activation](#1-installation--activation)
- [2. Meeting the editor](#2-meeting-the-editor)
- [3. Creating a timeline](#3-creating-a-timeline)
- [4. Creating a character](#4-creating-a-character)
- [5. Adding the dialog to your game](#5-adding-the-dialog-to-your-game)

## 1. Installation & Activation

Dialogic 2 requires Godot 4.1 or higher. If you don't know what version you have installed, take a look at the bottom of your Godot Editor.

Let's install Dialogic 2:
- Download the ZIP file here from your wanted Dialogic version: [GitHub Dialogic Releases](https://github.com/coppolaemilio/dialogic/releases).
- Extract the `addons` folder from this ZIP-file, it contains Dialogic.
- Move the `addons` folder to your Dialogic project folder.

Now, let's verify you have correctly installed Dialogic:
- You have this folder path `res://addons/dialogic`
- Head to `Project > Project Settings`
- Click the `Plugins` tab.
- Tick the `enabled` button next to Dialogic.
- Restart Godot

## 🚧How to install the latest WIP version🚧

> *Dialogic is constantly evolving. Oftentimes fixes for bugs or new features might only be available on the main branch. This is especially true during the alpha and beta phase. If you are interested in using the main branch it's easy to do so.*
> *Go to [the main page of the repository](https://github.com/coppolaemilio/dialogic) and click on the green `Code` button then presse the `Download ZIP` button. From there you can install that ZIP's content like a release.* 

## 2. Meeting the editor

You can now access the dialogic interface by clicking the new tab at the very top (next to 2D, 3D, Script and AssetLib).
![godot_main_tabs](/media/godot_main_tabs.png)

You will be greeted by the dialogic home screen. At the top you can see the different editor dialogic has, at the left the a sidebar that will contain recently used characters and timelines.

<img src="/media/editor_overview.png" width="600"/>

In the top right there are some helpful buttons:

- Add Timeline
- Add Character
- Reference Manager
- Play Timeline

We will start by using the first one.

## 3. Creating a timeline

To create a timeline you press the `Add Timeline`. You will need to select a folder to put the timeline in and enter a file name. Timelines will be saved as `*.dtl` files.

Once you hit `Save`, you can start adding events from the panel at the right of the editor.
<img src="/media/timeline_editor.png" width="600"/>

*Tip: You can learn more about each event and it's settings by right-clicking on an event and selecting `Documentation`.*

If you want, you can switch to the text editor by clicking on the `Text Editor` button at the top right. You can find out more about writing timelines in text format here: [Writing timelines in text format](./Timeline_Text_Syntax.md).

You can test the timeline by clicking the `Play Timeline` button at the top right.

## 4. Creating a character

To create a new character press the `Add Character` button on the top right. 

As for timelines, you need to select the place to save to and a name. 

⚠️*Important: This name (without .dch) is what will be saved whenever you use that character in a timeline and what you will have to write when referencing the character (e.g. `Emilio: This is a text event.`, if the file is named Emilio.dch). So make sure to give it a good name. You can change the name that will actually be displayed in game as the `display_name` property.*

Once your character is created, you will see the character editor. This editor has 4 main sections.
<img src="/media/character_editor.png" width="600"/>

You can learn more about portraits, custom portraits and the character settings in this tutorial: *[Characters & Portraits](/documentation/characters-and-portraits)*

## 5. Adding the dialog to your game

The last important step is to actually have this dialog show up in your game.

For that we need two things to happen: 

- A) having nodes that can display our timeline and 
- B) start the execution of the timeline.

Luckily for us, Dialogic provides a method that does both of those: `Dialogic.start(@timeline_name_or_path)`

*So code to start your dialog when an input is pressed could look like this:*

```gdscript
func _input(event:InputEvent):
    # check if a dialog is already running
    if Dialogic.current_timeline != null:
        return

    if event is InputEventKey and event.keycode == KEY_ENTER and event.pressed:
        Dialogic.start('chapterA')
        get_viewport().set_input_as_handled()
```

## You have gotten started!

Congratulations! You now know the basics of dialogic. There is much more to learn though. Here is a list of tutorials you might want to explore next:

- [Writing timelines in text format](./Timeline_Text_Syntax.md)
- [Characters and Portraits](/documentation/characters-and-portraits)
- [Creating timelines in code](/documentation/creating-timelines-in-code)
- [Designing your own layout scene](/documentation/dialogic-nodes)
