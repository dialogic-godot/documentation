![header_getting_started](/media/headers/autoadvance.png)

## What is Auto-Advance?

Auto-Advance is an experience-changing feature in Dialogic that allows players
to automatically progress through the timeline without requiring user input!\
It's particularly useful for providing a hands-free experience to your players,
offering an alternative to traditional "click-to-advance" methods in games.

You may also know this feature by the names "auto-forward" or simply "auto".

## How to use it?

Let's explore how you can enhance your player's experience with Auto-Advance,
taking into account their reading proficiency and the text's complexity.

### Text Settings

In Dialogic's Settings tab, under the Text section, you can find the
Auto-Advance settings.
![header_saving_loading](/media/auto_advance_settings.png)
Hover over the tooltip icons to learn more about each setting.

One critical setting is the "Additional Delay", which allows you to choose
between "Per Character" and "Per Word".\
These settings modify the pace at which text is displayed, adding extra delays
either on character or word count.


### Per Word vs. Per Character

Some languages, for instance Japanese, don't separate words by spaces.\
Dialogic uses the popular whitespace used by the space bar to determine when a
word ends and another begins.\
If you plan on providing multiple localisations, you can set both settings
via the API.

## Using the Auto-Advance API

With Dialogic's Auto-Advance API, you can effortlessly control and customise the Auto-Advance feature to suit your game's needs. Don't be intimidated; it's more straightforward than you might think!

### Auto-Advance Variables

The variables are used by Dialogic to decide how Auto-Advance must behave.\
You can access them via `Dialogic.Input.auto_advance`.

There are two types of variables:

- **Enable conditions**: `enabled_until_next_event`, `enabled_forced`, `enabled_until_user_input`
- **Behaviour changing**: `fixed_delay`, `per_word_delay`, `per_character_delay`, `await_playing_voice`, …

As long as one of the enable conditions is `true`, Auto-Advance will continue.
This allows stacking the reasons why Auto-Advance has been enabled.\
Imagine, the player enables Auto-Advance, but the Text event forces it on until the
next event.\
Thanks to the multiple enable conditions, if the player disables Auto-Advances,
it will still carry on until the next event.

You can turn any of the enable-variables to `true` activating Auto-Advance. If you have an Auto-Advance button, you can use the following code to enable the feature:

```gdscript
Dialogic.Input.auto_advance.enabled_until_user_input = true
```

#### Reading Speed

For Visual Novels, enabling players to set their text speed is a common practice.
To provide the same feature using Dialogic, use `Dialogic.Input.auto_advance.delay_modifier`.
This setting multiplies the total calculated Auto-Advance delay time. Faster readers may want a lower number.\

#### Ignored Characters

These characters will be ignored when calculating the text. This feature allows
you to further fine-tune your Auto-Advance experience. If you don't need it,
simply toggle it off.

### Auto-Advance via BBCode

BBCode tags can enable Auto-Advance via `[aa]` or `[aa = 10]`.\
This forces Auto-Advance to last at least until the next Text Timeline Event.\
If the BBCode provides a valid duration in seconds, Auto-Advance will wait for
this amount, ignoring `per_word_delay` and `per_character_delay`, but respecting `await_playing_voice`.

Alternatively, if you want to override the Auto-Advance time for the current
event only, add a `?` behind the duration: `[aa = 10?]`.

### Signal

Stay informed about changes in Auto-Advance's state by leveraging the
`Dialogic.Input.auto_advance.toggled` signal.

```gdscript
signal toggled(enabled: bool)
```

If you are interested in how Dialogic uses this signal internally, `Input` subsystem connects to this signal:

```gdscript
Dialogic.Input.autoadvance.toggled.connect(_on_autoadvance_toggled)
```

### API-only Variables

In order to keep things tidy, not all variables can be changed via Auto-Advance's settings page.\
The following variables can be accessed via code only.

#### Skipping Voice Clips

The `await_playing_voice` variable ensures that voice clips finish playing
before text advances.\
By default, Dialogic will let all voice clips finish, if you don't want this
behaviour, you can disable it via the API:

```gdscript
Dialogic.Input.auto_advance.await_playing_voice = false
```

#### Per Character and Per Word Delays

To accommodate languages without spaces between words, you can adjust the `per_word_delay` and `per_character_delay` variables using the API.\
 Here's an example of how to configure these settings in your script:

```gdscript
func _ready():
    # We can change the settings by directly writing to the returned dictionary.
    Dialogic.Input.auto_advance.per_word_delay = 0.3
    Dialogic.Input.auto_advance.per_character_delay = 0.1
```

Note, if you swap between languages, you'll need to update these settings
accordingly if you don't want languages with whitespaces to be affected by both.
