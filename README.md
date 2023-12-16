# Dialogic 2 - Documentation Repository

This repository contains the documentation of Dialogic 2.

It utilises [mdBook](https://rust-lang.github.io/mdBook) to generate and render the website.
If you find a mistake, please open an issue.

## Adding a new page
New pages should be added to the `documentation` folder. The `SUMMARY.md` file contains the table of contents displayed as a sidebar. Please add your new page to this file.

## Updating the website
The `md` files can be displayed in many applications supporting markdown. However, the website is generated using `mdBook`. The website utilises a build script to generate the website and push it to the `gh-pages` branch. On GitHub, these build scripts are called GitHub Actions.

## Book Structure
The `documentation` folder contains the book pages.

The `theme` folder overrides the [built-in](https://github.com/rust-lang/mdBook/tree/master/src/theme) `mdBook` style/theme files.

The `book.toml` contains the configuration of the documentation book.

A preprocessor decides how the book's chapters will be modified before building the final published book.\
The preprocessors are not part of the built-in feature set and were developed by other developers.\
They must be installed, see the [`.github/workflows/mdbook.yml`](https://github.com/dialogic-godot/documentation/blob/main/.github/workflows/mdbook.yml) for this.

## Run the documentation locally
To build the documentation, we need its software `mdBook`, which is written in the Rust Language

1. First, install Rust: https://www.rust-lang.org/tools/install
Open a new console, this allows `cargo` to function and makes the following commands possible.

2. Let's install `mdBook`: `cargo install mdbook`

3. We need to install the preprocessor for the admonish feature: `cargo install mdbook-admonish`

4. Finally, you can run this command inside this project's root: `mdbook serve --open`

The workflow is also described in the [.github/workflows/mdbook.yml](https://github.com/dialogic-godot/documentation/blob/main/.github/workflows/mdbook.yml) file.

## Admonish
The documentation supports admonish. We use a preprocessor for this.
You can create these by using the following syntax, using `info` as an example category:
````
```admonish info
The info text goes here.
```
````

Some available admonish categories: `info`, `warning`, `danger`, `tip`, `question`, `bug`, `example`, …

All admonish categories: https://tommilligan.github.io/mdbook-admonish/reference.html#directivese

## Chapter Banners
Each page has its own header banner.\
These can be created via this syntax:
```html
<div class="header-banner ocean">
     <div class="header-label ocean">Creating Extensions</div>
</div>
```

Alongside `ocean`, you can find the rest defined here: [header.css](https://github.com/dialogic-godot/documentation/blob/main/header.css).

## Table of Contents
The table of contents is generated automatically when you use the `[toc]` tag in your markdown file.\
Internally, this is invokes a preprocessor that generates the table of contents based on the headers below the tag.

This is the current style guide for our documentation:
```
## 📜 Content
[toc]
```