<div class="header-banner tropical">
     <div class="header-label tropical">Writing Text Events</div>
</div>

*Whether you write in the visual editor or text editor, inside texts you can use a bunch of special syntax to make them look and behave just the way you want.*

*Additionally, you can also use **BBCode,** about which you can learn more in the Godot docs: [BBCode in RichTextLabel](https://docs.godotengine.org/en/stable/tutorials/ui/bbcode_in_richtextlabel.html).*

## 📜 Content

[toc]

## What is a Text Effect?

A Text Effect (or text-tag) is a written command in the form of a special [BBCode](https://docs.godotengine.org/en/stable/tutorials/ui/bbcode_in_richtextlabel.html).
While Godot's BBCodes require a Rich Text Label, Dialogic's work inside the timeline's Text Events and do **not** use Godot's system for custom BBCode effects.

Dialogic's Text Effects permit you to control Auto-Advance (whether text continues automatically), waiting some time, awaiting your own signals, or changing the text speed.


## 1. Variables

You can use dialogic variables (and even autoload variables) in your text events easily. Learn more about how to do so here: [Variables](./variables.md)



---

## 2. Breaks and New Events

`[br]` Inserts a break into a text event.

`[n]` Seemingly starts a new event, requiring some sort of advancement (user input or auto-advance)

`[n+]` Requires some sort of advance (user input or auto-advance), but will append the following text to the previous without clearing the text box.

`[input]` Will simply await any input. As opposed to [n+], it is not breaking the text up into multiple sections and can thus be skipped. 



---

## 3. Speed & Pause effects

Text speed is a complicated topic, as it can be used in numerous ways. Dialogic has

- a **letter speed** that specifies the time to wait on each symbol when revealing

- a **speed multiplier** that will temporarily modify the letter and pause speed

- a **user speed multiplier setting** that will additionally modify letter and pause speed

##### 3.1 Letter Speed

The default letter speed can be changed in the text settings. It can be changed temporarily (it will reset before the next event) with these effects:

- `[lspeed=x]` Sets the letter speed to x in seconds (e.g., `[lspeed=0.1]`). *This is modified by the temporary speed multiplier and the user speed setting!*

- `[lspeed=x!]` Sets the letter speed to x in seconds. *This is **not multiplied** with the speed multipliers!*

- `[lspeed]` Resets the letter speed.

##### 3.2. Temporary Speed Multiplier

The speed multiplier is 1 by default, so it has no effect. It can be changed temporarily (it will reset before the next event) with these effects:

- `[speed=x]` Sets the speed to x. As this will multiply the pause length or letter delay, higher values will result in a slower reveal, and lower values will result in a faster reveal. 0 will instantly reveal the text.

- `[speed]` Resets the speed multiplier to 1.

##### 3.3 Pauses

You can pause the reveal with these effects:

- `[pause=x]` Pauses the reveal for x seconds (e.g., `[pause=0.2]`). *This is modified by the temporary speed multiplier and the user speed setting!*

- `[pause=x!]` Pauses the reveal for x seconds. *This is **not multiplied** with the speed multipliers!*

Related to this are **Auto-Pauses**, which can be configured in the text settings to insert pause effects after certain symbols. This can be used to easily alter the flow of punctuation. 

##### 3.4 User Speed multiplier setting

Oftentimes, you might want to expose the reveal speed as a setting to the player. To easily allow this, you can use the `"text_speed"` setting. 

You can access it via the Settings subsystem `Dialogic.Settings.text_speed = 0.5`. This should enable you to implement a speed slider in your settings

```admonish
Settings of the settings subsystem are automatically saved by dialogic and loaded back even across game-sessions! So you might want to reset this on game start if you don't want that.  ---
```



---

## 4. Random selection

If a text is encountered multiple times during your game, it might be nice to vary it a bit. For this, the random selection modifier allows you to insert only one option from a list like this:

- `<Option 1/Option 2/Option 3>` Inserts one of the options (separated with /) into the text.
  
  - E.g.: `<Hi/Hello/Howdy> <my friend/dude/bro>, how are you doing?`



---

## 5. Signal effect

If you want to notify/activate something outside Dialogic in the middle of a text event, you can use the `[signal=arg]` effect. It will trigger the `Dialogic.text_signal` signal with the given argument as a string. Learn more about the signal: [Dialogic Signals](./dialogic-signals.md)



---

## 6. Portrait & Mood effects

You can change the portrait or typing mood of the speaker with these effects:

- `[portrait=name]` Changes the portrait of the speaker to the portrait with the given name.

- `[mood=name]` Changes the typing mood to the one with the given name.

---

# 7. Auto-Advance

There are the following text effects to control Auto-Advance:

- `[aa]` enables the Auto-Advance for the *current* text event.
- `[aa=time]` enables Auto-Advance after a fixed delay of `time` seconds; four seconds before Auto-Advance continues: `[aa=4]`
- `[aa=time?]` changes the fixed delay for the current text event but does not enable Auto-Advance.

