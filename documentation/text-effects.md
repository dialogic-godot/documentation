<div class="header-banner tropical">
     <div class="header-label tropical">Text Effects</div>
</div>

*Text effects are tags that define a position in text and an action that happens, when that position is reached during the reveal of the text. Many text effects take an additional argument. They are useful to change the behaviour of the text revealing (e.g. speed, pauses, skipping, etc.) or to react to specific moments in the text (signal, changing the speakers portrait or sound mood).*

## 📜 Content
[toc]

## Splitting Events

### Effect: New Event

**Syntax:** `[n]` / `[n+]`

Visually starts a new event, requiring manual advancement by the user or by the Auto-Advance system.

The variant with the `+` will append the following text to the previous without clearing the text box.

### Effect: Input

**Syntax:** `[input]` 

Will simply await any input when reached. As opposed to [n+], it is not breaking the text up into multiple sections and can thus be skipped. 

---

## Speeds & Pauses

Text speed is a complicated topic, as it can be used in numerous ways. Dialogic has

- a **letter speed** (specifies the time to wait on each symbol)

- a **speed multiplier** (modifies the letter and pause speed, resets every event)

- a **text speed setting** (also modifies letter and pause speed)

---

### Letter Speed

The letter speed defines the time (in seconds) that each letter takes to be revealed. The default can be changed in the text settings. It can be changed temporarily (it will reset before the next event) with these effects:

#### Effect: Setting Letter Speed

**Syntax:** `[lspeed=x]` / `[lspeed]` / `[lspeed=x!]` 

Sets the letter speed to x in seconds or resets to the default if no x is given. By default the speed is multiplied with both the temporary speed multiplier and the text speed setting. If you put a `!` behind the time (e.g. `[lspeed=0.1!]`) then this is not the case.

---

### Temporary Speed Multiplier

The speed multiplier is 1 by default, so it has no effect. It can be changed temporarily (it will reset before the next event) with these effects:

#### Speed Multiplier Effect

**Syntax:** `[speed=x]` / `[speed]`

Sets the temporary speed multiplier to x or 1 if nothing is given. As this will multiply the pause length and letter speed, a bigger number means a slower reveal, a smaller number means a faster reveal and 0 means an instant reveal.

---

### Pauses Effect

**Syntax:** `[pause=x]` / `[pause=x!]` 

Pauses the reveal for x seconds (e.g., `[pause=0.2]`). 

By default this duration will be multiplied with the temporary speed multipler and the text speed setting multiplier. If you put a `!` behind the time (e.g. `[pause=0.2!]`) then this is not the case. 

*Related to this are **Auto-Pauses**, which can be configured in the text settings to insert pause effects after certain symbols. This can be used to easily alter the flow of punctuation.*

---

### Multiplier "Text Speed" (Dialogic Setting)

This is a `Dialogic Setting` so something that can be changed in-game via the Settings subsystem and is stored automatically and globally.

It defaults to 1 (no effect) and can be used to add a reveal speed setting to your games option menu.

You can access it via the Settings subsystem `Dialogic.Settings.text_speed = 0.5`. This should enable you to implement a speed slider in your settings

---

## Signal Effect

**Syntax:** `[signal=arg]`

Emits the `Dialogic.text_signal` signal with the given argument. Useful if you want something to happen at a specific moment during the text. Learn more about the signal: [Dialogic Signals](./dialogic-signals.md)

---

## Portrait & Type Sound Mood Effects

### Portrait Effect

**Syntax:** `[portrait=name]`

Changes the portrait of the speaker to the portrait with the given name.

### Type Sound Mood Effect

**Syntax:** `[mood=name]`

Changes the typing mood to the one with the given name.

### Extra Data Effect

**Syntax:** `[extra_data=value]`

Changes the extra data of the speaker to the given value.

---

## Auto-Advance Effect

**Syntax:** `[aa]` / `[aa=x]` / `[aa=x?]`

Enables the Auto-Advance for the *current* text event. 

A time x (in seconds) can be given to set the Auto-Advance time. This time is absolute and overwrites the more relative "per word" or "per letter" settings. 

If the time is given with a `?` then it will *only* set the time and *not* enable Auto-Advance. This is useful if the player can freely enable/disable Auto-Advance and you just want to define a different Auto-Advance time for this event, but not change it's state. 

---

## No Skip Effect

**Syntax:** `[ns]` / `[ns=x]`

This effect temporarily (for this event) disables text skipping *and* manual advance and enables Auto-Advance with the given time x (in seconds).
