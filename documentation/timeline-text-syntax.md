<div class="header-banner dawn">
     <div class="header-label dawn">Timeline Text Syntax</div>
</div>

*Timelines are saved in a text format, which means that you can use any text-editing software to edit and create them. The built-in text editor provides useful autocompletion and syntax highlighting.*

*For Dialogic to register your timeline file, it has to use the `.dtl` extension!*

## 📜 Content

[toc]

## About short code events

Most events follow a shortcodes-like style:

```dtl
[background path="res://icon.png" fade="1.0"]
```

The order of the parameters is not relevant, but they have to be separated by at least one space. All parameters, regardless of type, have to be contained in double quotation marks.

To find all the parameters you can use on each event, check out their documentation by searching for their class in the Godot Help or this documentation.

## About special events

Some events have a custom syntax to make writing them easier. This includes:

### Text Event

```dtl
A wonderful text event, said by noone in particular.

Emilio: Hello and welcome!

Emilio (excited): I'm excited cann you tell?

Emilio: This is a text event with \
multiple lines. Isn't that great? It is!
```

Ending a text event with `\` will make it include the next line as well.

### Character event

```dtl
join Emilio (happy) center [animation="Bounce In"]

leave Emilio [animation="Bounce Out" length="0.3"]

update Emilio (excited) left [animation="Tada" wait="true" repeat="3" move_time="0.3"]
```

*Check the [Character Event](./event-character.md) documentation for more information and examples.*

### Choice event

The `|` can be used to put logic behind the choice option.

```dtl
- Yes
- No | [if {John.Relationship} > 23]
- Maybe | [if {Stats.Charisma} > 10] [else="disable" alt_text="Maybe [too insecure]"]
```

### Condition event

```dtl
if {Player.Wisdom} > 3:
    # dialogics syntax is indentation based!
elif {Player.Health} <= 10:
    # some events
else:
    #...
```

### Set Variable event

```dtl
set {MyVariable} += 10
```

Supported Operators are =, += , -= , *=, /=

### Comment event

```dtl
# Some comment
```

### Label event

```dtl
label LabelIdentifier

# a label with a display name
label LabelIdentifier (Display Name)
```

### Jump event

```dtl
jump LabelIdentifier

# Jump to a label in another timeline
jump TimelineName/LabelIdentifier

# Jump to the beginning of another timeline
jump TimelineName/
```

### Return event

```dtl
return
```

### Do/Call event

```dtl
do Autoload.method("argument")
```

## About indentation

Timelines use TAB indentation to know what events belong to a choice or condition block. Only changes in indentation are considered, so it doesn't really matter how much you indent, as long as you are consistent within one block.

## Example timeline

```dtl
[background path="res://assets/backgrounds/dialogic_factory.png"]

join Jowan left
Jowan (excited): Hello and welcome to[portrait=confused]...[pause=0.5] Wait? What is this?

join Emilio (happy) right
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

- How to reach the moon | [if {Player.Name} == "NASA"]
    Jowan (angry): NASA! It's you again. This is for making dialogs!\
    Please ask someone else about the moon!.
    
    jump WhatAbout

- How to write timelines in text format
    Jowan: Oh, well it's pretty intuitive.[pause= 0.2][portrait=questioning] I hope.
    
    Emilio: Let's hope it's easy as well.

[end_timeline]
```
