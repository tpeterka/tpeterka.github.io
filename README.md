# Project websites

These websites are created with a variety of web tools---node, jade, and markdown---all to avoid having to write html. The jade files are used to render html (i.e., generate html files with the same base name) when running make. The markdown files contain most of the textual content, and jade includes them during the rendering. This project can be used as a template for other websites simply by replacing or customizing the content to suit a particular need.

The steps to build and run the example are below.

# Install dependencies

- [node.js](https://nodejs.org/) (Needed for jade)
- npm (Should be included with node)
- [jade](http://jade-lang.com/) (The replacement for html)
- [jquery.js](https://jquery.com/) (Used for the main menu bar; you may substitute your favorite tool)

Use npm to customize the local install:

```sudo npm install```

This will create a `node_modules` directory; please do not add this directory in git. These are not source files and should remain unversioned.

# Customize the content

- add new jade files to the `TARGETS` in `Makefile`
- add new markdown files with text
- include markdown files in jade files

# Build the website

Run

```make```

This will render all the html pages. The home page is `index.html`.

# Commit and push to github.io

The website will appear [here](http://tpeterka.github.io/maui-project/).
