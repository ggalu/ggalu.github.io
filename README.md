# Website of the Gips-Schüle Chair for Sustainable Systems Engineering

This repository holds the source of the website of the Gips-Schüle Chair for Sustainable Systems
Engineering at INATECH, University of Freiburg. GitHub Pages builds and serves it at
<https://ggalu.github.io> whenever a commit is pushed to the `main` branch.

The site is a static Jekyll site. It uses the documentation theme
[millidocs](https://github.com/alexander-heimbuch/millidocs) by Alexander Heimbuch, which is
available under the MIT licence (see `LICENSE.md`). The theme files are copied into this
repository (`_layouts/`, `_includes/`, `_sass/`, `assets/`), so changes to the look of the site
are made there.

## Editing the content

Each page is a Markdown file in the root directory. A page appears in the sidebar menu when its
front matter has a `navigation` entry. The menu is sorted by this number, so each page needs its
own number. If two pages share a number, their order in the menu is not defined. The numeric
prefixes of the file names only order the files in the directory and have no effect on the menu.

```yaml
---
layout: page
title: "Research: Example"
navigation: 12
---
```

Images are stored under `images/` (`people/`, `equipment/`, `research/<topic>/`, `logo/`), and
PDF documents with their preview images under `pdfs/`. Images are sized with kramdown attribute
lists, for example `![Name](/images/people/Name.jpg){: height="160" }`. A figure with a caption
is written as a one-column table, with the image in the header row and the caption in italics
below it.

## Previewing locally

With Ruby and Bundler installed, run `make install` once and then `make dev`. This serves the
site at <http://localhost:4000> and rebuilds it when a file changes. The build output in `_site/`
is not committed, because GitHub Pages builds the site itself.
