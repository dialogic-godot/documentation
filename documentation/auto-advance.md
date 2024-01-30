<div class="header-banner purple">
     <div class="header-label purple">Auto-Advance</div>
</div>

*Auto-Advance allows you to advance the timeline without user input.*

## 📜 Content
[toc]

## 1. What is Auto-Advance?

Auto-Advance is an experience-changing feature in Dialogic that allows players to automatically progress through the timeline without requiring user input!
It's particularly useful for providing a hands-free experience to your players, offering an alternative to traditional "click-to-advance" methods in games.

You may also know this feature by the names "auto-forward" or simply "auto".

---

## 2. Main Settings

In Dialogic's Settings tab, under the Text section, you can find the main Auto-Advance settings. Hover over the tooltip icons to learn more about each setting.
![header_saving_loading](media/auto_advance_settings.png)

#### 2.1 Additional Delay

One critical setting is the `Additional Delay`, which allows you to choose between **Per Character** and **Per Word**. These settings modify the pace at which text is displayed, adding extra delays either on character or word count.

Some languages, for instance Japanese, don't separate words by spaces. Dialogic uses the popular whitespace used by the spacebar to determine when a word ends and another begins. If you plan on providing multiple localisations, you can set both settings via the API.

##### Ignored Characters

These characters will be ignored when counting the characters. This feature allows you to further fine-tune your Auto-Advance experience. If you don't need it, simply toggle it off.

---

## 3. Changing Auto-Advance from code

Dialogic's Auto-Advance class can be easily accessed via the Inputs subsystem and allows you to change Auto-Advance during your game. It also has a number of settings not exposed to the dialogic interface.

All of this functionality lives in `Dialogic.Inputs.auto_advance` an `DialogicAutoAdvance` object.

### 3.1 Settings/Properties

There are two types of settings/properties:

#### Enable conditions

- `enabled_until_next_event: bool`
- `enabled_forced: bool`
- `enabled_until_user_input: bool`

As long as one of the enable conditions is `true`, Auto-Advance will continue.
This allows stacking the reasons why Auto-Advance has been enabled. Imagine, the player enables Auto-Advance, but the Text event forces it on until the next event.

Thanks to the multiple enable conditions, if the player disables Auto-Advances,
it will still carry on until the next event.

You can turn any of the enable-variables to `true` to enable Auto-Advance. If you have an Auto-Advance button, you can use the following code to enable the feature:

```gdscript
Dialogic.Inputs.auto_advance.enabled_until_user_input = true
```

#### Behaviour changing settings

- `fixed_delay: float` *Same as the base delay in the Settings*
- `per_word_delay: float` *Additional delay multiplied by the word count*
- `per_character_delay: float` *Additional delay multiplied by character count*
- `await_playing_voice: bool` *If true (by default) Auto-Advance will wait until voice lines have finished*

##### Per Character and Per Word Delays

You can see that using these properties you can have both per word and character delays which add up.

To accommodate languages without spaces between words, you can adjust the `per_word_delay` and `per_character_delay` variables when changing language.

Here's an example of how to configure these settings in your script:

```gdscript
# We can change the settings by directly writing to the returned dictionary.
Dialogic.Inputs.auto_advance.per_word_delay = 0.3
Dialogic.Inputs.auto_advance.per_character_delay = 0.1
```

### 3.2 Toggled Signal

If you want to be informed about changes in Auto-Advance's state, you can use the
`Dialogic.Inputs.auto_advance.toggled` signal.

```gdscript
signal toggled(enabled: bool)
```

If you are interested in how Dialogic uses this signal internally, the `Inputs` subsystem connects to this signal:

```gdscript
Dialogic.Inputs.autoadvance.toggled.connect(_on_autoadvance_toggled)
```

---

## 4. Modifying the reading speed

For Visual Novels, enabling players to set their text speed is a common practice.
To provide the same feature using Dialogic, consider setting `Dialogic.Settings.autoadvance_delay_modifier`.

This setting, located within `Dialogic.Settings`, allows you to fine-tune the
delay modifier, multiplying "Additional Delay".
By default, if this value is not set, Dialogic uses a multiplier of 1, causing
no change to the delay.

```admonish
Every setting added to `Dialogic.Settings` is automatically saved and loaded by Dialogic for the *player*.
```

## 5. Auto-Advance Text-Effect

By writing `[aa]` or `[aa = 2]` in your text, you can temporarily enable Auto-Advance in a text event and override the delay.

- `[aa]` enables Auto-Advance until (at least) the next text event

- `[aa=2]` enables Auto-Advance and sets the delay to 2 seconds.
  
  - This ignores `per_word_delay` and `per_character_delay` but respects `await_playing_voice`.

- `[aa=2?]` does **not** enable Auto-Advance but sets the time to 2 seconds if Auto-Advance is already enabled.
