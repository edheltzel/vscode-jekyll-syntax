# <a href="http://jekyllrb.com" title="Jekyll" target="_blank"><img src="https://raw.githubusercontent.com/ginfuru/vscode-jekyll-syntax/master/images/jekyll-logo.png" atl="Jekyll Logo" width="250"></a> syntax package for Visual Studio Code.

[![GitHub release](https://img.shields.io/github/release/ginfuru/vscode-jekyll-syntax.svg)](https://github.com/ginfuru/vscode-jekyll-syntax/releases)

### Inspired by [jekyll-atom](https://github.com/Arcath/jekyll-atom)

So this plugin was inspired by [@Arcath](https://github.com/Arcath)'s Atom plugin. So the roadmap will be to add the same _"grammars"_ available for Atom inside of Visual Studio Code. 

### Forked from [vscode-liquid](https://github.com/GingerBear/vscode-liquid)

I'm using this as a basis to add Jekyll specific syntax highlighting support - for those curious as to why a new plugin... well that's because I plan on adding more that just front-matter support.

### Using Emmet 

If you want to use Emmet with `Jekyll (HTML)` you'll need to add the below to your users settings or workspace settings _(the `scss` part is optional)_: 

```yaml
  "emmet.includeLanguages":{
    "jekyll": "html",
    "scss": "css"
  }
```



### Theme support

~~Front-Matter support in VSCode color schemes is limited, currently, but hopefully that changes over time. You can check out the two VSCode color themes/schemes below to see the improvements:~~ **With the edition of the include `source.yaml`** color scheme/theme support is pretty universal.

* **Better Solarized Dark**
  *  [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=ginfuru.ginfuru-better-solarized-dark-theme)
  *  [Repo](https://github.com/ginfuru/vscode-better-solarized-dark)
* **One Dark Rain Coat**
  *  [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=ginfuru.ginfuru-onedark-raincoat-theme)
  *  [Repo](https://github.com/ginfuru/vscode-onedark-raincoat)

If you'd like to add support to your color scheme add the following to your color schemes `.json` file

```json
    {
      "name": "Jekyll Tags Front Matter",
      "scope": [
        "punctuation.output.jekyll",
        "punctuation.tag.jekyll",
        "frontmatter.jekyll"
      ],
      "settings": {
        "foreground": "#SOME_COLOR_YOU_LINK"
      }
    },
```
**OR**
```json
    {
      "name": "Jekyll Tags",
      "scope": [
        "punctuation.output.jekyll",
        "punctuation.tag.jekyll"
      ],
      "settings": {
        "foreground": "#SOME_COLOR_YOU_LINK"
      }
    },
    {
      "name": "Jekyll Front Matter",
      "scope": [
        "frontmatter.jekyll"
      ],
      "settings": {
        "foreground": "#SOME_COLOR_YOU_LINK"
      }
    },
```
### TODO:

- [ ] add pictures
- [ ] add Jekyll JSON
- [ ] add Jekyll XML 
