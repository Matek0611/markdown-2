# GitHub User Content Stylesheets

Stylesheets for rendering GitHub Flavored Markdown, including syntax highlighted code snippets (powered by Pygments).



## SCSS and CSS

The GitHub user content stylesheets ship in two formats, CSS and SCSS.

### CSS

* `user-content.css` — Compiled CSS file ready to drop into any environment. Contains both Markdown and syntax stylesheets.
* `user-content.min.css` — Minified version of `user-content.css`

### SCSS

* `markdown.scss` — Source SCSS file for rendering markdown
* `user-content.scss` — `@imports` both of the above. If you import this file, you do not need to import the others.



## Development

The stylesheets are written in SCSS and compiled to regular CSS. Also included is a [Gruntfile](Gruntfile.js) for local project development.

1. Install `grunt-cli` globally with `npm install -g grunt-cli`.
2. Navigate to the root `/user-content` directory, then run `npm install` to install the necessary dependencies.
3. Done! Now you can run `grunt` from the command line to compile SCSS to CSS.

**Unfamiliar with `npm`? Don't have node installed?** That's a-okay. npm stands for [node packaged modules](http://npmjs.org/) and is a way to manage development dependencies through node.js. [Download and install node.js](http://nodejs.org/download/) before proceeding.



## Versioning

For transparency into our release cycle and in striving to maintain backward compatibility, the this project is maintained under the Semantic Versioning guidelines.

Releases will be numbered with the following format:

`<major>.<minor>.<patch>`

And constructed with the following guidelines:

- Breaking backward compatibility **bumps the major** while resetting minor and patch
- New additions without breaking backward compatibility **bumps the minor** while resetting the patch
- Bug fixes and misc changes **bumps only the patch**

For more information on SemVer, please visit <http://semver.org/>.



## License

Copyright 2014 GitHub, Inc. Released under [MIT license](LICENSE.md).
