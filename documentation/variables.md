<div class="header-banner tropical">
     <div class="header-label tropical">Variables</div>
</div>

*Variables are a good way to keep track of all kinds of things during your game.
Dialogic has an easy-to-use and beginner-friendly variable system built in. However, Dialogic allows you to use outside variables (or Autoload Singletons) just as easily.
You can also access the Dialogic variables from outside scripts.*

To fully utilize these variables, this page contains all you need to know.

## 📜 Content
[toc]

## 1. The Dialogic variable editor

Dialogic variables can be set up in the "Variables" tab. Each variable consists of a name and an initial default value.

Variables can be grouped together in folders, which just have a name.

Important: Inside a folder, no item (variable or folder) can have the same name.

---

## 2. Using variables in the timeline

### 2.1 Variables in texts

In text events, you can insert the value of a dialogic variable by typing `{variable_name}`.
If your dialogic variable is inside a folder (or multiple folders), you have to specify the whole name separated with dots: `{MyFolder.variable_name}` or `{FolderA.FolderB.variable_name}`

If you want to use a variable from an Autoload write `{AutoloadName.variable}`.
This syntax also allows calling methods on that autoload. Whatever is returned from the method is inserted into the text: `{Autoload.get_random_name()}`

You can even do simple operations inside the brackets: `{{Player.Health}/10.0+2}`

### 2.2 Conditions

One of the main uses for variables is in conditions: `if`, `elif`, or conditions on choices.

##### Conditions: Visual Editor

In the visual editor, you can simply select the variable from the dropdown and compare it to a value of your choice. If you need something more complex, click the `<E>` button and use the syntax described below.

##### Conditions: Text syntax

In conditions, you can use all the same tricks as in text events and a couple more:

- Accessing autoloads: `Autoload.property`
  
  - In these conditions, Autoloads don't have to be wrapped in `{}` brackets.*

- Using autoload methods: `Autoload.check_info("Argument", false)`

  - A condition always results in a boolean at the end, using the same rules as GDScript for type conversion.

- Using variables and typical boolean operators (`==`, `!=`, `<`, `>`, `<=`, `>=`, `not`, `and`, `or`, brackets):

  - `{Player.Health} > 5 or {Player.Luck} > randi()%10`

### 2.3 Set Variable event

You can change variables in a timeline with the set variable event. This can set dialogic variables as well as autoload variables.

##### Set Variable: Visual Editor

In the visual editor, you can simply select a variable and a value. You can also set the value of an Autoload variable by typing `Autoload.variable` in directly into the variable field and submitting with `Enter` (there is no auto-completion).

The value that it will be set to can be a

- string,

- number (float or int),

- value of another variable,

- complex expression,

- random number

**Complex Expression** allows you to use the full range of possibilities. Behind the scenes, all of these types are expressions; the distinction is only made for a simpler UI.

Expressions follow the syntax described below.

##### Set Variable: Text syntax

The set variable event has a special syntax to make it easy to write and read:

```dtl
set {variable_name} = 20

set {MyFolder.variable} += 2

set Autoload.property = "Hello World"

set {Player.Health} += range(10,20).pick_random()

set Autoload.health = {Player.Health} + 2
```

The value is parsed as an expression, similar to what is done with {expressions} inside text events or in conditions. All the same can be done here as well, the only difference is that it won't be converted to string/bool.

### 2.4 Text Input event

A special kind of set variable event is the `Text Input` event, which allows you to capture a text input the player makes in a variable.

---

## 3. Using variables for other cool stuff

#### 3.1 Variables as character names

A character `Display Name` can be a variable. That is the best way to control that character's name during the game. To achieve this, just type `{MyVariableName}` in the display name field in the character editor.

#### 3.2 Variables in glossaries

You can use variables in glossary titles, texts and extras. This is the best way to control the text during the game. You can do all the same things as in the text event.

---

## 4. Using variables outside Dialogic

You might want to access variables from scripts outside dialogic.

You can do so with direct access:

```gdscript
Dialogic.VAR.my_variable = 20
print(Dialogic.VAR.Group.other_variable)
```

You can also do so by string:

```gdscript
Dialogic.VAR.set('my_variable', 20)
print(Dialogic.VAR.get('Group').get('my_variable'))
```

> [!WARNING]
> Variables are only accessible after the Dialogic autoload is ready, so do not use them before your nodes are ready either!


Folders (as well as the root "folder") have some methods that might be useful:

- `folders()` lists all folders in this folder (not strings but `FolderObjects`)

- `variables(@absolute)` lists the names of all the variables in that folder

- `has(@variable_name)` returns true if such a variable exists

This allows you to do fancy stuff like this:

```gdscript
var location = Dialogic.VAR.Towns.folders().pick_random().variables().pick_random()
```

Could pick a random house/place if your variables are set up like this:

```
Towns (folder)

   - Town A (folder)

      - CharacterAHouse

      - CharacterBHouse

      - Church

      - School

  - Town B (folder)

      - CharacterCHouse

      - CharacterDHouse

      - University

      - Park
```

Dialogic.VAR also has:

- `Dialogic.VAR.reset(@variable_path="")` resets the given variable or all variables if none is specified

- `Dialogic.VAR.parse_variables(@string)` returns the given string with variables replaced. This is what is used by the text event, etc.
