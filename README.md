# Dialogic 2 - Documentation Repository

This repository contains the documentation of Dialogic 2.

It utilises [mdBook](https://rust-lang.github.io/mdBook) to generate and render the website.
If you find a mistake, please open an issue.

# Adding a new page
New pages should be added to the `src` folder. The `SUMMARY.md` file contains the table of contents displayed as sidebar. Please add your new page to this file.

# Updating the website
The `md` files can be displayed in many applications supporting markdown. However, the website is generated using `mdBook`. The website utilises a build script to generate the website and push it to the `gh-pages` branch. On GitHub, these build scripts are called GitHub Actions.

# Structure
The `src` folder will be used to build the website. The `book` folder contains build files and should not be edited manually.

# Admonish
The documentation supports admonish.
You can create these by using the following syntax using `info` as example category:
````
```admonish info
The info text goes here.
```
````

Some available admonish categories: `info`, `warning`, `danger`, `tip`, `question`, `bug`, `example`, …

All admonish categories: https://tommilligan.github.io/mdbook-admonish/reference.html#directivese
