---
title: Styles & Layouts
---

![header_style-editor](/media/headers/styles_and_layouts.png)

<details open>
<summary>📜 Content</summary>

- [1. Styles & Layouts](#1-Styles--Layouts)

- [2. The style editor](#2-The-style-editor)
  
  </details>

# 1. Styles & Layouts

- A **style** is a combination of a layout scene (preset or custom) and a set of settings. 
- A **layout** is a scene that can display dialog ingame.

Dialogic comes with some **preset layouts**, but you can create your own using DialogicNodes. Learn more about [custom layouts here](./Dialogic_Nodes.md).

![layout_presets](/media/layout_presets.png)

*You can add more presets with extensions. Feel free to share cool layouts you've made via the [discord](https://discord.gg/2hHQzkf2pX).*

# 2. The style editor

The style editor allows you to create and edit styles. By default you only have the `Default` style that uses the VisualNovel layout.

<img src="/media/style_editor.png" width="600"/>

### Style list

The style list section lets you:

- add new styles
- duplicate styles
- add a new style that inherits the current one
- delete styles
- mark the current style as default

### Changing the Layout

You can change the layout the current style uses by clicking `Change` next to the layout thumbnail. This will open a layout selection page:

<img src="/media/style_editor_layout_selection.png" width="600"/>

- Select Custom will allow you to select a scene from your project
- Clicking a preset will show info about that preset and allow you to select it

*If your style inherits from another style, the layout is determined by the "parent"-style and cannot be changed.*

### Inheritance

You can set a style to inherit from another one. A style will inherit the layout and the settings from it's parent style.

### Settings

Layouts can expose settings to the editor. These can easily be changed for each style and allow customizing a style. The presets each come with different settings.
