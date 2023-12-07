![header_text_syntax](media/headers/text_syntax.png)

Timelines are saved in a text format, which means that you can use any text-editing software to edit and create them. The built in text editor provides useful autocompletion and syntax highlighting.
📜
*Info: For dialogic to register your timeline file, it has to use the `.dtl` extension!*

<details open>
<summary>📜 Content</summary>

- [About shortcode events](#about-shortcode-events)

- [About special events](#about-special-events)

- [About Indentation](#about-indentation)

- [Example Timeline](#Example-timeline)

  </details>

## About shortcode events

Most events follow a shortcodes-like style:

```dtl
[background path="res://icon.png" fade="1.0"]
```

The order of the parameters does not matter, but they have to be separated by at least one space. All parameters regardless of type have to be contained in double quotation marks.

To find all of the parameters you can use on each event, check out their documentation by searching for their class in the godot help or this documentation.

## About special events

Some events have a custom syntax, to make writing them easier. This includes:

- Character event:

  - `join Emilio (happy) 3 [animation="Bounce In"]`
  - `leave Emilio [animation="Bounce Out" length="0.3"]`
  - `update Emilio (excited) 4 [animation="Tada" wait="true" repeat="3" move_time="0.3"]`

- Text event: 

  - `A wonderful text event, said by noone in particular.`
  - `Emilio (excited): Hello and welcome!`
  - Ending a text event with \ will make it include the next line as well.

- Choice event:

  - `- I don't know about that`
  - `- Yes [if {John.Relationship} > 23]`
  - `- Sure, I'm the great wizard [if {Stats.Charisma} > 10] [else="disable" alt_text="I'm the great wizard [to insecure]"]`

- Condition event:

  - `if {Player.Wisdom} > 3:`
  - `elif {Player.Health} <= 10:`
  - `else:`

- Set Variable event:

  - `set {MyVariable} += 10`
  - Supported Operators are =, += , -= , *=, /=

- Comment event:

  - `# Todo: Finnish this!!!!`

- Label event:

  - `label MyLabelName`

- Jump event:

  - `jump MyLabelName`
  - `jump TimelineName/` # the slash is mandatory to clarify this is a timeline not a label
  - `jump TimelineName/LabelName`

- Return event:

  - `return`

## About indentation

Timelines use TAB indentation to know what events belong to a choice or condition block. Only changes in indentation are considered, so it doesn't really matter how much you indent as long as you are consistent within one block.

## Example timeline

```dtl
[background path="res://assets/backgroudns/dialogic_factory.png"]

join Jowan 4
jowan (exited): Hello and welcome to[portrait=confused]...[pause=0.5] Wait? What is this?

join Emilio (happy) 1
Emilio: Well, this is is the example timeline.

Jowan: I thought this was a cool new feature?

Emilio: Nah, sorry.

Jowan (sad): It's okay.

# Some choices jump back to this
label WhatAbout

Jowan (default): So what should this example be about?
- How to bake cookies
    Emilio (confused): Wait that hasn't to do with dialogic?!
    jump WhatAbout

- How to reach the moon [if {Player.Name} == "NASA"]
    Jowan (angry): NASA! It's you again. This is for making dialogs!\
    Please ask someone else about the moon!.
    
    jump WhatAbout

- How to write timelines in text format
    Jowan: Oh, well it's pretty intuitive.[pause= 0.2][portrait=questioning] I hope.
    
    Emilio: Let's hope it's easy as well.

[end_timeline]
```
