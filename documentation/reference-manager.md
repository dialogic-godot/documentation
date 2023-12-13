<div class="header-banner purple">
     <div class="header-label purple">Reference Manager</div>
</div>

*The reference manager allows fixing broken references and renaming unique resource identifiers.*

## 📜 Content

- [1. What kind of references are we talking about?](#1-what-kind-of-references-are-we-talking-about)
- [2. Broken references](#2-broken-references)
- [3. Unique Identifiers](#3-unique-identifiers)

## 1. What kind of references are we talking about?

Dialogic timelines are saved in text-syntax that often favors being readable over being specific: You do not have to specify the exact character resource every time you reference a character. 

To do this, dialogic assigns each of its resources (*timelines and characters*) a `unique identifier` string. This string is initially based on the file name but can be whatever; the only important thing is: not two resources (of the same type) can have the same identifier. 

There is some other name based references in dialogic, notably *portraits* and *variables*. 

Dialogic provides tools to edit unique identifiers and also easily fix any `broken references` if you choose to rename something after having already used it in a timeline. These tools live in the Reference Manager which can be accessed via the Link button in the toolbar.

---

## 2. Broken references

The first tab allows you to fix references after you renamed something. 

Dialogic will sometimes send you here. In those cases it has usually already added some renames that you should check for. 

Simply click `Check Selected` which will scan all timelines for the references in the list above. Check if the results look like they contain the thing you want to actually replace. If not just uncheck them. Then click `Replace`.

```admonish
This performs a destructive operation on all affected timelines. It can not be easily undone if it goes wrong.
It usually works fine, but if you use custom regexes you should be pretty careful. 
If you use version control, this would be the perfect moment to commit! 
```

The tool will automatically remove any resolved (or irrelevant) renames from the list when you close the window.

#### 2.1 Custom replacements (Advanced)

This tool can also be used to manually replace something. This is useful if dialogic didn't correctly pick up on a rename or you would like to replace some other string in all timelines. 

This can be done by clicking the `Plus button`. 

If you select `Pure Text` you can enter a custom term or regex. The regex can contain a `(?<replace>something)` group if you would like to not replace the whole result.

Any of the other options (`Variable`, `Portrait`, `Character`, `Timeline`) will use a custom regex specialized for those types.

You can also limit a search to only lines related to a specific character (useful for portraits). 

Lastly click `Add`. An entry will be added to the list. You can then continue like with automatically added entries. 

--- 

## 3. Unique identifiers

Thes second tab allows you to change the unique identifiers for your characters and timelines.  

You can simply double click an identifier or use the Pen button on the left.

No two identifiers in the same category can be the same.

Renaming any identifier will automatically add an entry to the "Broken References" tab which you can use to check if this rename broke anything.
