<div class="header-banner blurple">
     <div class="header-label blurple">Frequently Asked Questions</div>
</div>

## 📜 Content
[toc]

## May I use Dialogic in one of my projects?

Yes, you may use Dialogic to make any kind of game - even commercial ones!
The project is developed under the [MIT License](https://github.com/coppolaemilio/dialogic/blob/master/LICENSE). All we ask is that you please remember to credit us in your project!

If you want to be featured on the "Made with Dialogic"-page, get in touch with us on [Emilio's Discord server](https://discord.gg/2hHQzkf2pX)!

## How can I change the input?

Dialogic uses a Godot `InputAction` for the so-called "Input Action". By default, this is the `dialogic_default_action` which is automatically created when enabling the plugin. You can either edit this action or use a different input action by changing the setting in the dialogic settings Text section.

## How to make the dialog show up in the game?

The easiest way to make the dialog appear in your game is to call `Dialogic.start("res://path/to/timeline.dtl")` in your game. This will both create a [layout scene](styles-and-layouts.md) and start the timeline.

## Why are my portraits not showing up?

When using the Visual Novel layout, to make the characters show up on the screen, you need to make them join your current scene using the Character event (Join mode).

## Why isn't this part of Godot?

> The plugin is cool! Why is it not shipped with Godot?

I see numerous people saying that the plugin should come with Godot, but I believe this should stay as a plugin since most of the people making games won't be using it. I'm flattered by your comments, but this will remain a plugin :)

## How do I start and stop background music?

Use a `Music` event to set a resource and then cancel it with a `Music` event with no resource.

![header_faq](/media/faq/background_music_toggling.png)

This example will fade in the music over 4 seconds and then fade it out over 5 seconds.

## How do I find the current speaker or its portrait index?

The following snippet will give you the current speaker and its portrait information, including the index.

```gdscript
var current_speaker: DialogicCharacter = Dialogic.Text.get_current_speaker()
var portrait_info := Dialogic.Portraits.get_character_info(current_speaker)
var speaker_portrait_index := portrait_info.position_index
```
