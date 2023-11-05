---
title: Translation
---

![header_getting_started](/media/headers/autoskip.png)

## What is Translation?

Translation is a Godot and Dialogic 2 feature, that allows you to translate your game into multiple languages.

Sometimes, the word Localisation is used as well.
The concept of Localisation is a way broader and often provides very specific regional consideration for each target region.

## How create Translation?

In Dialogic, Translation is a feature that can be enabled via the Settings tab, under the Translation section.

First, you can set the time each event is allowed to take via the Text settings page inside Dialogic.

![translation_settings](/media/translation/translation_settings.png)

### Setting up Translation

Ensure you tick the "Enable Translation" checkbox to enable the feature.

Then, you will have to pick a default locale. This locale will be used as a fallback, if no translation is available for the current locale.

The translation file mode allows you to store all your timelines into one file (Per Project) or into multiple files (Per Timeline).

Setting up a translation folder is a good idea, it keeps your project clean and allows you to easily find your translation files.

### Writing Translation

First of all, you will need to have a timeline file. Dialogic will automatically find and generate CSV files for you after you hit the "Update CSV files" button.

The CSV format is very simple and has a great variety of support. You can open it with any spreadsheet software, like Excel or Google Sheets. Even VSCode offers extensions to edit the file.\
The gist of CSV files is that each line represents a row and each column is separated by a comma.

Once Dialogic has generated the CSV file, it may look like this:

```csv
keys,en
Text/1/text,Hello World!"
```

The `keys` are locales, the `en` is the locale code for English, if you chose a different default locale, it will be different.

You can add a new language for your game by adding a new column.

```csv
keys,en,ja
Text/1/text,Hello World!,こんにちは世界！
```

That's it! You can now hit "Collect translation" and Dialogic will generate a translation file for you.\
The translation file is a specific Godot file. Here is their official documentation: [Internationalising games](https://docs.godotengine.org/en/stable/tutorials/i18n/internationalizing_games.html)

### The Translation Workflow

From now on, whenever you change the CSV file, you can hit "Collect translation" again and Dialogic will update the translation file for you.\
Additionally, if you are done editing your timeline, you will have to hit "Update CSV files" again to update the CSV file.

In order to verify, whether your timeline has been properly translated, you can switch into the  timeline Text editor.

```
Character: Hello world! #id:14
Do you like Visual Novels? #id:15
- Yes, I do! #id:16
- No, I love them! #id:17
That's the spirit! #id:18
```

The `#id` tags at the end of each Text Event are the translation IDs. They won't be visible during text display, however, you can be rest assured that Dialogic has inserted them into a CSV file.

## How to test Translation?

If everything went well, you can select a different locale in the "Testing locale" dropdown.\
Hit "Play Timeline" or "Run Project" and take a look at the translated text.\
This setting is editor-only and may not work in exported projects.

## Scripting API

The translation process itself is handled by Godot!

In order to change the locale when your game is exported, use the Godot API method on the [TranslationServer](https://docs.godotengine.org/en/stable/classes/class_translationserver.html#translationserver) class:


```gdscript
# Japanese's language code is "ja"
TranslationServer.set_locale("ja")
```