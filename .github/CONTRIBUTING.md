# Contributing

Contributions are welcome!

## Adding a resource

Most awesome lists are written in a single long Markdown file (see [awesome-list](https://github.com/topics/awesome-list)). However, in this repository each resource is described in a separate Markdown file (see [content/items](../content/items)). The frontmatter is used to provide data about the resource, while the body can contain a long description. The prototype of the frontmatter is shown in [template.md](../template.md).

Further guidelines:

* Add one resource/file per Pull Request (PR) and explain why it is awesome.
* Keep descriptions in the frontmatter concise.
* See list of defined categories in [config.yml](../config.yml).
  * Add a new category if needed. If done, a description of the category must be included.
* Regular chores:
  * Search previous suggestions before making a new one.
  * Check spelling and grammar.
  * Remove any trailing whitespace.
* An optional logo can be added under `static/logos`:
  * Size must be between 128x128 and 196x196 pixels (preferred).
  * The logo must be vertical/horizontal centered.
  * Use a white background with roundered corners (10%) if needed.
* Filenames must be lowercase.

## Modifying the site/theme

The website is built with [Hugo](https://github.com/gohugoio/hugo), using a theme based on [Bare Hugo](https://github.com/orf/bare-hugo-theme). The theme is a submodule of the `main`|`develop` branches. However, at the same time, the customized version is hosted in branch `theme` of this same repo. Hence, users willing to contribute to the theme need to:

- Clone this repo recursively, or `git submodule update --init --recursive`.
- Change directory to `themes/bare-hugo-theme`.
- Make changes, commit them and push a feature branch.
- Open a pull request against branch `theme`, NOT `main`|`develop`.
