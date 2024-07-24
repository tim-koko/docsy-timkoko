# Docsy Tim&Koko

Additions for the [docsy theme](https://github.com/google/docsy) for [Hugo](https://gohugo.io/), used for [tim&koko](https://tim-koko.ch) training content.
The docsy-timkoko theme inherites from the docsy theme through Hugo [Modules](https://gohugo.io/hugo-modules/use-modules/).

The theme adds the following to the standard docsy theme:

* brand colors scheme and fonts
* logo and favicons

## Installation

To add the docsy, docsy-plus and docsy-timkoko themes to an existing Hugo project, run the following commands from your project’s root directory:

```sh
hugo mod get github.com/acend/docsy-plus
hugo mod get github.com/tim-koko/docsy-timkoko
```

Reference both themes in your configuration.

Example config.toml:

```toml
[module]
  [module.hugoVersion]
    extended = true
    min = "0.100.0"
  [[module.imports]]
    path = "github.com/tim-koko/docsy-timkoko"
    disable = false
  [[module.imports]]
    path = "github.com/acend/docsy-plus"
    disable = false
```

Docsy itself is a dependency of docsy-plus
