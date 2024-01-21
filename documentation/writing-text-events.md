<div class="header-banner tropical">
     <div class="header-label tropical">Writing Text Events</div>
</div>

*Whether you write in the visual editor or text editor, inside of texts you can use a bunch of special syntax to make it look and behave just the way you want.*

*Additionally you can also use **BBCode** about which you can lear more in the godot docs: [BBCode in RichTextLabel](https://docs.godotengine.org/en/stable/tutorials/ui/bbcode_in_richtextlabel.html).*

## 📜 Content

[toc]

## 1. Variables

You can use dialogic variables (and even autoload variables) in your text events easily. Learn more about how to do so here: [Variables](./variables.md)



---

## 2. Breaks and New Events

`[br]` Inserts a break into a text event.

`[n]` Seemingly starts a new event, requiring some sort of advancement (user input or auto-advance)

`[n+]` Requires some sort of advance (user input or auto-advance) but will append the following text to the previous, without clearing the textbox.

`[input]` Will simply await any input. Differently then [n+] it is not breaking the text up into multiple sections and can thus be skipped. 



---

## 3. Speed & Pause effects

The text speed is a complicated topic as it can be used in numerous ways. Dialogic has

- a **letter speed** which specifies the time to wait on each symbol when revealing

- a **speed multiplier** which will temporarily modify the letter and pause speed

- a **user speed multiplier setting** which will additionally modify letter and pause speed

##### 3.1 Letter Speed

The defautlt letter speed can be changed in the text settings. It can be changed temporarily (will reset before the next event) with these effects:

- `[lspeed=x]` Sets the letter speed to x in seconds (e.g. `[lspeed=0.1]`). *This is modified by the temporary speed multiplier and the user speed setting!*

- `[lspeed=x!]` Sets the letter speed to x in seconds. *This is **not multiplied** with the speed multipliers!*

- `[lspeed]` Resets the letter speed.

##### 3.2. Temporary Speed Multiplier

The speed multiplier is 1 by default and so has no effect. It can be changed temporarily (will reset before the next event) with these effects:

- `[speed=x]` Sets the speed to x. As this will multiply the pause length or letter delay, higher values will result in a slower reveal and lower values in faster reveal. 0 will result in a instant reveal.

- `[speed]` Resets the speed multiplier to 1

##### 3.3 Pauses

You can pause the reveal with these effects:

- `[pause=x]` Pauses the reveal for x seconds (e.g. `[pause=0.2]`). *This is modified by the temporary speed multiplier and the user speed setting!*

- `[pause=x!]` Pauses the reveal for x seconds. *This is **not multiplied** with the speed multipliers!*

Related to this are **Auto-Pauses**, which can be configured in the text settings to insert pause effects after certain symbols. This can be used to easily alter the reveal-flow on punctuation. 

##### 3.4 User Speed multiplier setting

Oftentimes you might want to expose the reveal speed as a setting to the player. To easily allow this, you can use the `"text_speed"` setting. 

You can access it via the Settings subsystem `Dialogic.Settings.text_speed = 0.5`. This should enable you to implement a speed slider in your settings

```admonish
Settings of the settings subsystem are automatically saved by dialogic and loaded back even across game-sessions! So you might want to reset this on game start if you don't want that.  ---
```



---

## 4. Random selection

If a text is encountered multiple times during your game, it might be nice to vary it a bit. For this the random selection modifier allows you to insert only one option from a list like this:

- `<Option 1/Option 2/Option 3>` Inserts one of the options (seperated with /) into the text.
  
  - E.g.: `<Hi/Hello/Howdy> <my friend/dude/bro>, how are you doing?`



---

## 5. Signal effect

If you want to notify/activate something outside of dialogic in the middle of a text event, you can use the `[signal=arg]` effect. It will trigger the `Dialogic.text_signal` signal with the given argument as a string. Learn more about the signal: [Dialogic Signals](./dialogic-signals.md)



---

## 6. Portrait & Mood effects

You can change the portrait or typing mood of the speaker with these effects:

- `[portrait=name]` Changes the portrait of the speaker to the portrait with the given name.

- `[mood=name]` Changes the typing mood to the one with the given name.
