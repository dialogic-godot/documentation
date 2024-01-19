<div class="header-banner purple">
     <div class="header-label purple">Voice-Synced Text</div>
</div>

*Syncing text to character voices provides a unique reading experience.*

## 📜 Content
[toc]

## 1. What is voice-synced Text?

Voice-synced text is a feature in Dialogic that allows you to sync text to playing character voices.

This feature is perfect for visual novels, providing a lot of voice acting. \
The player may choose to use [Auto-Advance](auto-advance.md) to automatically progress through the timeline while syncing the text to the voice lines instead of letting the text prematurely appear.

In the end, this feature is a preference. Players may start reading slower and do not have to wait for voice lines to finish.

---

## 2. How do I enable the feature?

The voice-synced text feature must be enabled via the Dialogic API. Take a look at the following code:

```gdscript
Dialogic.Text.set_voice_synced_text(true)
```

We are suggesting the player decides whether they want this feature enabled.

---

## 3. Limitations

This feature is based on the length of the audio playing; it does not respect
the speech pattern of the voice line.

Auto-Pauses on letters will be ignored.
