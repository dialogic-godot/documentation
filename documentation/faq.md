# Frequently Asked Questions

![header_faq](/media/header_faq.png)

## May I use Dialogic in one of my projects?

*Yes, you may use Dialogic to make any kind of game - even commercial ones!
The project is developed under the [MIT License](https://github.com/coppolaemilio/dialogic/blob/master/LICENSE). All we ask is that you please remember to credit us in your project!*

*If you want to be featured on the made with dialogic page, get in touch with us on [emilios discord server](https://discord.gg/2hHQzkf2pX)!*

## How can I change the input?

*Dialogic uses a godot `InputAction` for the so called "Input Action". By default this is the `dialogic_default_action` which is automatically created when enabling the plugin. You can either edit this action or use a different input action by changing the setting in the dialogic settings Text section.*

## How to make dialog show up in game?

*The easiest way to make the dialog appear in your game is to call `Dialogic.start("res://path/to/timeline.dtl")` in your game. This will both instance a [layout scene](../Documentation/Styles_&_Layouts.md) and start the timeline.*

## Why are my portraits not showing up?

*When using the VisualNovel layout, in order to make the characters show up on the screen, you need to make them join your current scene using the Character event (Join mode).*

## Why isn't this part of godot?

*The plugin is cool! Why is it not shipped with Godot? I see a lot of people saying that the plugin should come with Godot, but I believe this should stay as a plugin since most of the people making games won't be using it. I'm flattered by your comments but this will remain a plugin :)*

## How do I start and stop background music?

Use a `Music` event setting a resource and then cancel it with a `Music` event with no resource.

![header_faq](/media/faq/background_music_toggling.png)

This example will fade-in the music over 4 seconds and then fade it out over 5 seconds.
