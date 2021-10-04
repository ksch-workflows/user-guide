# User Guide

This repository contains a scaffold for quickly creating new websites with the [Workshop Materials](https://github.com/experimental-software/workshop-materials) Hugo theme.


### Update dummy content

After cloning the repository, you to replace the dummy content from the template with the content of your workshop materials:

- [x] [Update license information](README.md#license)
- [ ] [Update dummy config](config.toml)
- [ ] [Update dummy home page text](content/_index.md)
- [x] [Update dummy subject](content/subject-one)
- [ ] [Add legal text to imprint](content/imprint.html)

## Development

### Run Hugo server

To a development server that always re-renders after every change, run the following command:

```
hugo server
```

### Build website

To generate the HTML for publication, run the following command:

```
hugo --destination docs/
```

## Content authoring

### Tutorials

#### Add a new tutorial

Run the following command to add a new presentation in Hugo's `content` directory:

```
hugo new --kind tutorial subject-two/my-tutorial
```

#### Content syntax

The presentations can be created using [Markdown](https://daringfireball.net/projects/markdown/) syntax.

#### Content syntax extensions

Along with the Markdown syntax, you can use the following custom [Hugo shortcodes](https://gohugo.io/content-management/shortcodes):

**Info callout box**

```
{{< info >}}
Lorem [impsum](https://example.com) dolor sit amet.
{{< /info >}}
```

**Tip callout box**

```
{{< tip >}}
Lorem [impsum](https://example.com) dolor sit amet.
{{< /tip >}}
```

**Warning callout box**

```
{{< warning >}}
Lorem [impsum](https://example.com) dolor sit amet.
{{< /warning >}}
```

### Presentations

#### Presentation syntax

The presentations can be created using plain HTML with the [reveal.js](https://revealjs.com/) syntax.

#### Add a new presentation

Run the following command to add a new presentation in Hugo's `content` directory:

```
hugo new --kind presentation subject-two/my-presentation
```

## References

- https://en.wikipedia.org/wiki/User_guide
- https://experimental-software.github.io/workshop-materials

## Credits

- The layout of the start page and the subject list pages is applied from a Bootstrap template by [Xiaoying Riley](https://themes.3rdwavemedia.com/) which is licensed under Creative Commons Attribution 3.0 License.
- The layout of the tutorial pages is inspired by [Google Codelabs](https://github.com/googlecodelabs/tools).
- The presentations are based on [reveal.js](https://revealjs.com/) which is licensed under the [MIT license](https://github.com/hakimel/reveal.js/blob/master/LICENSE).
- At various places of the website [Font Awesome](https://fontawesome.com/) icons are used.

## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
