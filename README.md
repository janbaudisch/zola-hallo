# Belarus Rust Community

Introduction page of community use static site engine [Zola][zola]. Based on [zola-hallo][zola-hallo] theme.

## Local start
> 1. Install Zola.
> 2. go into directory with project
> 3. zola serve

## Original

This is a port of the original [hallo-hugo][hallo-hugo] theme for Hugo ([License][upstream-license]).

## Installation

The easiest way to install this theme is to either clone it ...

```
git clone https://github.com/janbaudisch/zola-hallo.git themes/hallo
```

... or to use it as a submodule.

```
git submodule add https://github.com/janbaudisch/zola-hallo.git themes/hallo
```

Either way, you will have to enable the theme in your `config.toml`.

```toml
theme = "hallo"
```

### Introduction

The introduction text is made in `content/_index.md`.

## Options

See [`config.toml`][config] for an example configuration.

### Author

The given name will be used for the 'I am ...' text.

Default: `Hallo`

```toml
[extra.author]
name = "Hallo"
```

### Greeting

The string will be used as a greeting.

Default: `Hello!`

```toml
[extra]
greeting = "Hello!"
```

### `iam`

This variable defines the `I am` text, which you may want to swap out for another language.

Default: `I am`

```toml
[extra]
iam = "I am"
```

### Links

Links show up below the introduction. They are styled with [Font Awesome][fontawesome], you may optionally choose the iconset (default
is [brands][fontawesome-brands]).

```toml
[extra]
links = [
    { title = "E-Mail", url = "mailto:mail@example.org", iconset = "fas", icon = "envelope" },
    { title = "GitHub", url = "https://github.com", icon = "github" },
    { title = "Twitter", url = "https://twitter.com", icon = "twitter" }
]
```

### Theme

Change the colors used.

```toml
[extra.theme]
background = "#6FCDBD"
foreground = "#FFF" # text and portrait border
hover = "#333" # link hover
```

[zola]: https://www.getzola.org
[zola-hallo]: https://github.com/janbaudisch/zola-hallo
[hallo-hugo]: https://github.com/EmielH/hallo-hugo
[fontawesome]: https://fontawesome.com
[fontawesome-brands]: https://fontawesome.com/icons?d=gallery&s=brands&m=free
[upstream-license]: https://github.com/janbaudisch/zola-hallo/blob/master/upstream/LICENSE
[config]: https://github.com/janbaudisch/zola-hallo/blob/master/config.toml
