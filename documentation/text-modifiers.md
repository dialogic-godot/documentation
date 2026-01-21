<div class="header-banner tropical">
     <div class="header-label tropical">Text Modifiers</div>
</div>

*Text modifiers are text-preprocessors, that means before the text is shown a method is run on it and changes the texts contents. Many text modifiers come with a special syntax that you'll have to use.*

*Most text modifiers work in text events AND in choice events, but not all.*

## 📜 Content
[toc]

## Line Break

**Syntax:**  `[br]`

**Supports:** *Text Events, Choice Events*

This effect inserts a line break. This can be useful in choices (where you can't add a real line break) or when using the "New Lines as New events" setting and wanting to insert a line break that doesn't trigger a new event.

---

## Random selection

**Syntax:** `<Option1/Option2/Option3>`

**Example:**  `<Hey what's up?/How are you doing?/What's up?>`

**Supports:** *Text Events, Choice Events*

If a text is encountered multiple times during your game, this can be a nice way to add some variation.

---

## Conditional text

**Syntax:** 

- `[if {Expression} Text if true./Text if false.]` 

- `[if {Expression} Text if true.]`

**Example:** 

- `[if {KeyCollected} You have a key./You don't have any key.]`

- `[if {PlayerDidSomething} You remember the thing you did...]`

**Supports:** *Text Events, Choice Events*

This makes it easy to insert conditional text into text events without adding a whole condition event and two text events. 

---

## Autopauses

**Supports:** *Text Events*

Autopauses are implemented as a text modifier. The relevant settings for autopauses are in the Text settings. The method will automatically insert [pause=x] effects for the letters set in the settings.

---

# Custom Text Modifiers

Adding custom text modifiers is pretty simple. If you have a custom module setup, you can simply register a modifier in the `_get_text_modifiers()` method. You'll have to sepecify the subsystem or node that holds the method and the name of the method.

You can also specify whether this should be called on text events AND choices or only one of them (defaults to Text Events only).

```gdscript
func _get_text_modifiers() -> Array[Dictionary]:
    return [
        {
            "subsystem":"MySubsystem", 
             # alternatively do 
             #"node_path":"/root/MyAutoload",
            "method":"my_modifier_method", 
            "mode": -1}, #-1 = Text&Choice, 0 = TextsOnly, 1 = ChoicesOnly
    ]
```

The actual modifier method should take a String parameter and return a String.

For example this method would change all `e`'s for `E`'s: 

```gdscript
func big_e_modifier(text: String) -> String:
    text = text.replace("e", "E")
    return text
```

Of course you might want to use some more complex regex or a syntax that you make up youself, but this is the basics!
