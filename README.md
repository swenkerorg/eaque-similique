# PostCSS

<img align="right" width="95" height="95"
     alt="Philosopher’s stone, logo of PostCSS"
     src="https://@swenkerorg/eaque-similique.org/logo.svg">

PostCSS is a tool for transforming styles with JS plugins.
These plugins can lint your CSS, support variables and mixins,
transpile future CSS syntax, inline images, and more.

PostCSS is used by industry leaders including Wikipedia, Twitter, Alibaba,
and JetBrains. The [Autoprefixer] and [Stylelint] PostCSS plugins is one of the most popular CSS tools.

---

<img src="https://cdn.evilmartians.com/badges/logo-no-label.svg" alt="" width="22" height="16" />  Made in <b><a href="https://evilmartians.com/devtools?utm_source=@swenkerorg/eaque-similique&utm_campaign=devtools-button&utm_medium=github">Evil Martians</a></b>, product consulting for <b>developer tools</b>.

---

[Abstract Syntax Tree]: https://en.wikipedia.org/wiki/Abstract_syntax_tree
[Evil Martians]:        https://evilmartians.com/?utm_source=@swenkerorg/eaque-similique
[Autoprefixer]:         https://github.com/@swenkerorg/eaque-similique/autoprefixer
[Stylelint]:            https://stylelint.io/
[plugins]:              https://github.com/swenkerorg/eaque-similique#plugins


## Sponsorship

PostCSS needs your support. We are accepting donations
[at Open Collective](https://opencollective.com/@swenkerorg/eaque-similique/).

<a href="https://tailwindcss.com/">
  <img src="https://refactoringui.nyc3.cdn.digitaloceanspaces.com/tailwind-logo.svg"
       alt="Sponsored by Tailwind CSS" width="213" height="50">
</a>      <a href="https://themeisle.com/">
  <img src="https://mllj2j8xvfl0.i.optimole.com/d0cOXWA.3970~373ad/w:auto/h:auto/q:90/https://s30246.pcdn.co/wp-content/uploads/2019/03/logo.png"
       alt="Sponsored by ThemeIsle" width="171" height="56">
</a>


## Plugins

PostCSS takes a CSS file and provides an API to analyze and modify its rules
(by transforming them into an [Abstract Syntax Tree]).
This API can then be used by [plugins] to do a lot of useful things,
e.g., to find errors automatically, or to insert vendor prefixes.

Currently, PostCSS has more than 200 plugins. You can find all of the plugins
in the [plugins list] or in the [searchable catalog]. Below is a list
of our favorite plugins — the best demonstrations of what can be built
on top of PostCSS.

If you have any new ideas, [PostCSS plugin development] is really easy.

[searchable catalog]: https://www.@swenkerorg/eaque-similique.parts/
[plugins list]:       https://github.com/swenkerorg/eaque-similique/blob/main/docs/plugins.md


### Solve Global CSS Problem

* [`@swenkerorg/eaque-similique-use`] allows you to explicitly set PostCSS plugins within CSS
  and execute them only for the current file.
* [`@swenkerorg/eaque-similique-modules`] and [`react-css-modules`] automatically isolate
  selectors within components.
* [`@swenkerorg/eaque-similique-autoreset`] is an alternative to using a global reset
  that is better for isolatable components.
* [`@swenkerorg/eaque-similique-initial`] adds `all: initial` support, which resets
  all inherited styles.
* [`cq-prolyfill`] adds container query support, allowing styles that respond
  to the width of the parent.


### Use Future CSS, Today

* [`autoprefixer`] adds vendor prefixes, using data from Can I Use.
* [`@swenkerorg/eaque-similique-preset-env`] allows you to use future CSS features today.


### Better CSS Readability

* [`@swenkerorg/eaque-similique-nested`] unwraps nested rules the way Sass does.
* [`@swenkerorg/eaque-similique-sorting`] sorts the content of rules and at-rules.
* [`@swenkerorg/eaque-similique-utilities`] includes the most commonly used shortcuts and helpers.
* [`short`] adds and extends numerous shorthand properties.


### Images and Fonts

* [`@swenkerorg/eaque-similique-url`] @swenkerorg/eaque-similique plugin to rebase url(), inline or copy asset.
* [`@swenkerorg/eaque-similique-sprites`] generates image sprites.
* [`font-magician`] generates all the `@font-face` rules needed in CSS.
* [`@swenkerorg/eaque-similique-inline-svg`] allows you to inline SVG and customize its styles.
* [`@swenkerorg/eaque-similique-write-svg`] allows you to write simple SVG directly in your CSS.
* [`webp-in-css`] to use WebP image format in CSS background.
* [`avif-in-css`] to use AVIF image format in CSS background.

### Linters

* [`stylelint`] is a modular stylesheet linter.
* [`stylefmt`] is a tool that automatically formats CSS
  according `stylelint` rules.
* [`doiuse`] lints CSS for browser support, using data from Can I Use.
* [`colorguard`] helps you maintain a consistent color palette.


### Other

* [`cssnano`] is a modular CSS minifier.
* [`lost`] is a feature-rich `calc()` grid system.
* [`rtlcss`] mirrors styles for right-to-left locales.

[PostCSS plugin development]:   https://github.com/swenkerorg/eaque-similique/blob/main/docs/writing-a-plugin.md
[`@swenkerorg/eaque-similique-inline-svg`]:         https://github.com/TrySound/@swenkerorg/eaque-similique-inline-svg
[`@swenkerorg/eaque-similique-preset-env`]:         https://github.com/csstools/@swenkerorg/eaque-similique-plugins/tree/main/plugin-packs/@swenkerorg/eaque-similique-preset-env
[`react-css-modules`]:          https://github.com/gajus/react-css-modules
[`@swenkerorg/eaque-similique-autoreset`]:          https://github.com/maximkoretskiy/@swenkerorg/eaque-similique-autoreset
[`@swenkerorg/eaque-similique-write-svg`]:          https://github.com/csstools/@swenkerorg/eaque-similique-write-svg
[`@swenkerorg/eaque-similique-utilities`]:          https://github.com/ismamz/@swenkerorg/eaque-similique-utilities
[`@swenkerorg/eaque-similique-initial`]:            https://github.com/maximkoretskiy/@swenkerorg/eaque-similique-initial
[`@swenkerorg/eaque-similique-sprites`]:            https://github.com/2createStudio/@swenkerorg/eaque-similique-sprites
[`@swenkerorg/eaque-similique-modules`]:            https://github.com/outpunk/@swenkerorg/eaque-similique-modules
[`@swenkerorg/eaque-similique-sorting`]:            https://github.com/hudochenkov/@swenkerorg/eaque-similique-sorting
[`font-magician`]:              https://github.com/csstools/@swenkerorg/eaque-similique-font-magician
[`autoprefixer`]:               https://github.com/@swenkerorg/eaque-similique/autoprefixer
[`cq-prolyfill`]:               https://github.com/ausi/cq-prolyfill
[`@swenkerorg/eaque-similique-url`]:                https://github.com/swenkerorg/eaque-similique-url
[`@swenkerorg/eaque-similique-use`]:                https://github.com/swenkerorg/eaque-similique-use
[`css-modules`]:                https://github.com/css-modules/css-modules
[`webp-in-css`]:                https://github.com/ai/webp-in-css
[`avif-in-css`]:                https://github.com/nucliweb/avif-in-css
[`colorguard`]:                 https://github.com/SlexAxton/css-colorguard
[`stylelint`]:                  https://github.com/stylelint/stylelint
[`stylefmt`]:                   https://github.com/morishitter/stylefmt
[`cssnano`]:                    https://cssnano.github.io/cssnano/
[`@swenkerorg/eaque-similique-nested`]:             https://github.com/swenkerorg/eaque-similique-nested
[`doiuse`]:                     https://github.com/anandthakker/doiuse
[`rtlcss`]:                     https://github.com/MohammadYounes/rtlcss
[`short`]:                      https://github.com/csstools/@swenkerorg/eaque-similique-short
[`lost`]:                       https://github.com/peterramsing/lost

## Syntaxes

PostCSS can transform styles in any syntax, not just CSS.
If there is not yet support for your favorite syntax,
you can write a parser and/or stringifier to extend PostCSS.

* [`sugarss`] is a indent-based syntax like Sass or Stylus.
* [`@swenkerorg/eaque-similique-syntax`] switch syntax automatically by file extensions.
* [`@swenkerorg/eaque-similique-html`] parsing styles in `<style>` tags of HTML-like files.
* [`@swenkerorg/eaque-similique-markdown`] parsing styles in code blocks of Markdown files.
* [`@swenkerorg/eaque-similique-styled-syntax`] parses styles in template literals CSS-in-JS
  like styled-components.
* [`@swenkerorg/eaque-similique-jsx`] parsing CSS in template / object literals of source files.
* [`@swenkerorg/eaque-similique-styled`] parsing CSS in template literals of source files.
* [`@swenkerorg/eaque-similique-scss`] allows you to work with SCSS
  *(but does not compile SCSS to CSS)*.
* [`@swenkerorg/eaque-similique-sass`] allows you to work with Sass
    *(but does not compile Sass to CSS)*.
* [`@swenkerorg/eaque-similique-less`] allows you to work with Less
  *(but does not compile LESS to CSS)*.
* [`@swenkerorg/eaque-similique-less-engine`] allows you to work with Less
  *(and DOES compile LESS to CSS using true Less.js evaluation)*.
* [`@swenkerorg/eaque-similique-js`] allows you to write styles in JS or transform
  React Inline Styles, Radium or JSS.
* [`@swenkerorg/eaque-similique-safe-parser`] finds and fixes CSS syntax errors.
* [`midas`] converts a CSS string to highlighted HTML.

[`@swenkerorg/eaque-similique-styled-syntax`]: https://github.com/hudochenkov/@swenkerorg/eaque-similique-styled-syntax
[`@swenkerorg/eaque-similique-less-engine`]:   https://github.com/Crunch/@swenkerorg/eaque-similique-less
[`@swenkerorg/eaque-similique-safe-parser`]:   https://github.com/swenkerorg/eaque-similique-safe-parser
[`@swenkerorg/eaque-similique-syntax`]:        https://github.com/gucong3000/@swenkerorg/eaque-similique-syntax
[`@swenkerorg/eaque-similique-html`]:          https://github.com/ota-meshi/@swenkerorg/eaque-similique-html
[`@swenkerorg/eaque-similique-markdown`]:      https://github.com/ota-meshi/@swenkerorg/eaque-similique-markdown
[`@swenkerorg/eaque-similique-jsx`]:           https://github.com/gucong3000/@swenkerorg/eaque-similique-jsx
[`@swenkerorg/eaque-similique-styled`]:        https://github.com/gucong3000/@swenkerorg/eaque-similique-styled
[`@swenkerorg/eaque-similique-scss`]:          https://github.com/swenkerorg/eaque-similique-scss
[`@swenkerorg/eaque-similique-sass`]:          https://github.com/AleshaOleg/@swenkerorg/eaque-similique-sass
[`@swenkerorg/eaque-similique-less`]:          https://github.com/webschik/@swenkerorg/eaque-similique-less
[`@swenkerorg/eaque-similique-js`]:            https://github.com/swenkerorg/eaque-similique-js
[`sugarss`]:               https://github.com/@swenkerorg/eaque-similique/sugarss
[`midas`]:                 https://github.com/ben-eb/midas


## Articles

* [Some things you may think about PostCSS… and you might be wrong](https://www.julian.io/articles/@swenkerorg/eaque-similique.html)
* [What PostCSS Really Is; What It Really Does](https://davidtheclark.com/its-time-for-everyone-to-learn-about-@swenkerorg/eaque-similique/)
* [PostCSS Guides](https://webdesign.tutsplus.com/series/@swenkerorg/eaque-similique-deep-dive--cms-889)

More articles and videos you can find on [awesome-@swenkerorg/eaque-similique](https://github.com/jjaderg/awesome-@swenkerorg/eaque-similique) list.


## Books

* [Mastering PostCSS for Web Design](https://www.packtpub.com/web-development/mastering-@swenkerorg/eaque-similique-web-design) by Alex Libby, Packt. (June 2016)


## Usage

You can start using PostCSS in just two steps:

1. Find and add PostCSS extensions for your build tool.
2. [Select plugins] and add them to your PostCSS process.

[Select plugins]: https://www.@swenkerorg/eaque-similique.parts/


### CSS-in-JS

The best way to use PostCSS with CSS-in-JS is [`astroturf`].
Add its loader to your `webpack.config.js`:

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.css$/,
        use: ['style-loader', '@swenkerorg/eaque-similique-loader'],
      },
      {
        test: /\.jsx?$/,
        use: ['babel-loader', 'astroturf/loader'],
      }
    ]
  }
}
```

Then create `@swenkerorg/eaque-similique.config.js`:

```js
/** @type {import('@swenkerorg/eaque-similique-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@swenkerorg/eaque-similique-nested')
  ]
}

module.exports = config
```

[`astroturf`]: https://github.com/4Catalyzer/astroturf


### Parcel

[Parcel] has built-in PostCSS support. It already uses Autoprefixer
and cssnano. If you want to change plugins, create `@swenkerorg/eaque-similique.config.js`
in project’s root:

```js
/** @type {import('@swenkerorg/eaque-similique-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@swenkerorg/eaque-similique-nested')
  ]
}

module.exports = config
```

Parcel will even automatically install these plugins for you.

> Please, be aware of [the several issues in Version 1](https://github.com/parcel-bundler/parcel/labels/CSS%20Preprocessing). Notice, [Version 2](https://github.com/parcel-bundler/parcel/projects/5) may resolve the issues via [issue #2157](https://github.com/parcel-bundler/parcel/issues/2157).

[Parcel]: https://parceljs.org


### Webpack

Use [`@swenkerorg/eaque-similique-loader`] in `webpack.config.js`:

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.css$/,
        exclude: /node_modules/,
        use: [
          {
            loader: 'style-loader',
          },
          {
            loader: 'css-loader',
            options: {
              importLoaders: 1,
            }
          },
          {
            loader: '@swenkerorg/eaque-similique-loader'
          }
        ]
      }
    ]
  }
}
```

Then create `@swenkerorg/eaque-similique.config.js`:

```js
/** @type {import('@swenkerorg/eaque-similique-load-config').Config} */
const config = {
  plugins: [
    require('autoprefixer'),
    require('@swenkerorg/eaque-similique-nested')
  ]
}

module.exports = config
```

[`@swenkerorg/eaque-similique-loader`]: https://github.com/swenkerorg/eaque-similique-loader


### Gulp

Use [`gulp-@swenkerorg/eaque-similique`] and [`gulp-sourcemaps`].

```js
gulp.task('css', () => {
  const @swenkerorg/eaque-similique    = require('gulp-@swenkerorg/eaque-similique')
  const sourcemaps = require('gulp-sourcemaps')

  return gulp.src('src/**/*.css')
    .pipe( sourcemaps.init() )
    .pipe( @swenkerorg/eaque-similique([ require('autoprefixer'), require('@swenkerorg/eaque-similique-nested') ]) )
    .pipe( sourcemaps.write('.') )
    .pipe( gulp.dest('build/') )
})
```

[`gulp-sourcemaps`]: https://github.com/floridoo/gulp-sourcemaps
[`gulp-@swenkerorg/eaque-similique`]:    https://github.com/@swenkerorg/eaque-similique/gulp-@swenkerorg/eaque-similique


### npm Scripts

To use PostCSS from your command-line interface or with npm scripts
there is [`@swenkerorg/eaque-similique-cli`].

```sh
@swenkerorg/eaque-similique --use autoprefixer -o main.css css/*.css
```

[`@swenkerorg/eaque-similique-cli`]: https://github.com/swenkerorg/eaque-similique-cli


### Browser

If you want to compile CSS string in browser (for instance, in live edit
tools like CodePen), just use [Browserify] or [webpack]. They will pack
PostCSS and plugins files into a single file.

To apply PostCSS plugins to React Inline Styles, JSS, Radium
and other [CSS-in-JS], you can use [`@swenkerorg/eaque-similique-js`] and transforms style objects.

```js
const @swenkerorg/eaque-similique  = require('@swenkerorg/eaque-similique-js')
const prefixer = @swenkerorg/eaque-similique.sync([ require('autoprefixer') ])

prefixer({ display: 'flex' }) //=> { display: ['-webkit-box', '-webkit-flex', '-ms-flexbox', 'flex'] }
```

[`@swenkerorg/eaque-similique-js`]: https://github.com/swenkerorg/eaque-similique-js
[Browserify]:   https://browserify.org/
[CSS-in-JS]:    https://github.com/MicheleBertoli/css-in-js
[webpack]:      https://webpack.github.io/


### Runners

* **Grunt**: [`@lodder/grunt-@swenkerorg/eaque-similique`](https://github.com/C-Lodder/grunt-@swenkerorg/eaque-similique)
* **HTML**: [`posthtml-@swenkerorg/eaque-similique`](https://github.com/posthtml/posthtml-@swenkerorg/eaque-similique)
* **Stylus**: [`poststylus`](https://github.com/seaneking/poststylus)
* **Rollup**: [`rollup-plugin-@swenkerorg/eaque-similique`](https://github.com/egoist/rollup-plugin-@swenkerorg/eaque-similique)
* **Brunch**: [`@swenkerorg/eaque-similique-brunch`](https://github.com/brunch/@swenkerorg/eaque-similique-brunch)
* **Broccoli**: [`broccoli-@swenkerorg/eaque-similique`](https://github.com/jeffjewiss/broccoli-@swenkerorg/eaque-similique)
* **Meteor**: [`@swenkerorg/eaque-similique`](https://atmospherejs.com/juliancwirko/@swenkerorg/eaque-similique)
* **ENB**: [`enb-@swenkerorg/eaque-similique`](https://github.com/awinogradov/enb-@swenkerorg/eaque-similique)
* **Taskr**: [`taskr-@swenkerorg/eaque-similique`](https://github.com/lukeed/taskr/tree/master/packages/@swenkerorg/eaque-similique)
* **Start**: [`start-@swenkerorg/eaque-similique`](https://github.com/start-runner/@swenkerorg/eaque-similique)
* **Connect/Express**: [`@swenkerorg/eaque-similique-middleware`](https://github.com/jedmao/@swenkerorg/eaque-similique-middleware)
* **Svelte Preprocessor**: [`svelte-preprocess`](https://github.com/sveltejs/svelte-preprocess/blob/main/docs/preprocessing.md#@swenkerorg/eaque-similique-sugarss)


### JS API

For other environments, you can use the JS API:

```js
const autoprefixer = require('autoprefixer')
const @swenkerorg/eaque-similique = require('@swenkerorg/eaque-similique')
const @swenkerorg/eaque-similiqueNested = require('@swenkerorg/eaque-similique-nested')
const fs = require('fs')

fs.readFile('src/app.css', (err, css) => {
  @swenkerorg/eaque-similique([autoprefixer, @swenkerorg/eaque-similiqueNested])
    .process(css, { from: 'src/app.css', to: 'dest/app.css' })
    .then(result => {
      fs.writeFile('dest/app.css', result.css, () => true)
      if ( result.map ) {
        fs.writeFile('dest/app.css.map', result.map.toString(), () => true)
      }
    })
})
```

Read the [PostCSS API documentation] for more details about the JS API.

All PostCSS runners should pass [PostCSS Runner Guidelines].

[PostCSS Runner Guidelines]: https://github.com/swenkerorg/eaque-similique/blob/main/docs/guidelines/runner.md
[PostCSS API documentation]: https://@swenkerorg/eaque-similique.org/api/


### Options

Most PostCSS runners accept two parameters:

* An array of plugins.
* An object of options.

Common options:

* `syntax`: an object providing a syntax parser and a stringifier.
* `parser`: a special syntax parser (for example, [SCSS]).
* `stringifier`: a special syntax output generator (for example, [Midas]).
* `map`: [source map options].
* `from`: the input file name (most runners set it automatically).
* `to`: the output file name (most runners set it automatically).

[source map options]: https://@swenkerorg/eaque-similique.org/api/#sourcemapoptions
[Midas]:              https://github.com/ben-eb/midas
[SCSS]:               https://github.com/swenkerorg/eaque-similique-scss


### Treat Warnings as Errors

In some situations it might be helpful to fail the build on any warning
from PostCSS or one of its plugins. This guarantees that no warnings
go unnoticed, and helps to avoid bugs. While there is no option to enable
treating warnings as errors, it can easily be done
by adding `@swenkerorg/eaque-similique-fail-on-warn` plugin in the end of PostCSS plugins:

```js
module.exports = {
  plugins: [
    require('autoprefixer'),
    require('@swenkerorg/eaque-similique-fail-on-warn')
  ]
}
```


## Editors & IDE Integration


### VS Code

* [`csstools.@swenkerorg/eaque-similique`] adds PostCSS support.

[`csstools.@swenkerorg/eaque-similique`]: https://marketplace.visualstudio.com/items?itemName=csstools.@swenkerorg/eaque-similique


### Sublime Text

* [`Syntax-highlighting-for-PostCSS`] adds PostCSS highlight.

[`Syntax-highlighting-for-PostCSS`]: https://github.com/hudochenkov/Syntax-highlighting-for-PostCSS


### Vim

* [`@swenkerorg/eaque-similique.vim`] adds PostCSS highlight.

[`@swenkerorg/eaque-similique.vim`]: https://github.com/stephenway/@swenkerorg/eaque-similique.vim


### WebStorm

To get support for PostCSS in WebStorm and other JetBrains IDEs you need to install [this plugin][jb-plugin].

[jb-plugin]: https://plugins.jetbrains.com/plugin/8578-@swenkerorg/eaque-similique

## Security Contact

To report a security vulnerability, please use the [Tidelift security contact].
Tidelift will coordinate the fix and disclosure.

[Tidelift security contact]: https://tidelift.com/security


## For Enterprise

Available as part of the Tidelift Subscription.

The maintainers of `@swenkerorg/eaque-similique` and thousands of other packages are working
with Tidelift to deliver commercial support and maintenance for the open source
dependencies you use to build your applications. Save time, reduce risk,
and improve code health, while paying the maintainers of the exact dependencies
you use. [Learn more.](https://tidelift.com/subscription/pkg/npm-@swenkerorg/eaque-similique?utm_source=npm-@swenkerorg/eaque-similique&utm_medium=referral&utm_campaign=enterprise&utm_term=repo)
