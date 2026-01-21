<div class="header-banner pineapple">
     <div class="header-label pineapple">Glossary</div>
</div>

*This page explains how the built-in glossary feature can be utilized.*

## 📜 Content
[toc]

## 1. What is a glossary?

A glossary is a collection of terms with their definitions. It's a great way to keep track of your game's lore, characters, and more.

Some Visual Novels use a glossary to explain terms that may be unfamiliar to the player. For example, if your game is set in a fantasy world, you may want to explain the unique species that live in your world.

### 1.1 What does a Dialogic glossary do?

If a glossary contains keys, Dialogic will automatically use the `name` and `alternatives` properties of each
glossary entry to highlight them and provide a tooltip with the definition if hovered over.

## 2. How do I translate glossaries?

Take a look at [Translating Glossaries](translation.md#25-translating-glossaries) for more information.

## 3. Implementation

> [!NOTE]
> This section is aimed at programmers who may want to understand how the glossaries work under the hood.


A glossary is a text resource file (`tres`) and after each change to the
glossary, it has to be saved to the disk or the changes won't persist.

Furthermore, it has an `entries` property, containing an `Array` of
`Dictionary`s, whereas each `Dictionary` represents a glossary entry.

### 3.1 Translation ID

Once translated, each entry will have a unique `_translation_id`.\
The `_translation_id` will be added to `_translation_keys` glossary property,
mapping glossary name properties
to their entry array index.


### 3.2 Alias Keys

An entry key is a unique identifier for a glossary entry, either a name, an
alternative (alias), or an entry translation ID (CSV key).

The aliases are used to map the entry to the true glossary entry key, allowing the code
to map the glossary word to its glossary entry.

Additionally, the entry's translation ID allows the code to map a translated glossary
word to its translation ID and then to the glossary entry using the `_translation_keys`. \
The glossary entry IDs are combined, using the glossary ID and then the entry ID.
This matches the translation CSV keys for translated glossaries:
`Glossary/3b/6c/name`.


### 3.2 Accessing glossary properties

As a rule of thumb, if you want to access the glossary from code, do not access
the `_` prefixed aforementioned properties: `_translation_id`,
`_translation_keys`. They may change over the course of Dialogic's
development.

Instead, look for the helper methods on `DialogicGlossary`.


### 3.3 How do I get all glossary paths?

You can use the following project setting to get all glossary files:
```gdscript
var glossary_paths: Array[String] = ProjectSettings.get_setting('dialogic/glossary/glossary_files', [])
```
