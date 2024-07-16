<div class="header-banner tropical">
     <div class="header-label tropical">Writing Texts</div>
</div>

*When writing texts in text events or choices, you can utilize many systems to tweak the behaviour, content and styling of the texts.*
## 📜 Content

[toc]

## BBCode

In Text events you can use BBCode tags, that allow you to style your text: from bold, italics and underlines to colors, fonts, images, and crazy wave effects. Learn more in the Godot docs: [BBCode in RichTextLabel](https://docs.godotengine.org/en/stable/tutorials/ui/bbcode_in_richtextlabel.html).
If you need BBCode on the choice buttons, you will have to use custom choice buttons that use RichTextLabel to display their text! 

## Variables/Expressions

Anything in `{`curly brackets`}` will be considered an expression. It will be evaluated when the text is shown and the result will be inserted. This could be a simple **dialogic variable** or a **variable on an autoload**. Learn more on the [Variables page](./variables.md).

## Text modifiers

Text modifiers range from simple inserts like `[br]` (to insert a line break) to `<random/selection>` (selects a random option) or conditional texts `[if {Expression} Show if true./Else show this.]` (prints one of the text based on the result of the expression).

You can find a full list of the text modifiers here: [Text Modifiers](./text-modifiers.md)

## Text Effects

Text effects look similar to bbcode, but usually have an effect that happens when the text-revealing reaches that point. That could be `[pause=x]` (pauses x seconds), `[speed=x]` (changes the speed of revealing), or `[signal=x]` (emits the Dialogic.text_signal with the argument x).

You can find a list of all the text effects here: [Text Effects](./text-effects.md)
