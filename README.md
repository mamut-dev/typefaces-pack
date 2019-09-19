# @typefaces-pack

NPM packages for open source typographic fonts, which facilitates the self-management of web fonts inspired by repositories of [KyleAMathews - typefaces](https://github.com/KyleAMathews/typefaces).

## [@KyleAMathews](https://github.com/KyleAMathews)

- Self-hosting is _significantly faster_. Loading a typeface from Google
  Fonts or other hosted font service adds _an extra (blocking) network
  request_. [In my
  testing](https://github.com/reactiflux/reactiflux.com/pull/21), I’ve
  found replacing Google Fonts with a self-hosted font can improve a
  site’s speedindex by ~300 miliseconds on desktop and 1+ seconds on 3g.
  This is a big deal.
- Your _fonts load offline_. It’s annoying to start working on a web
  project on the train or airplane and see your interface screwed up
  because you can’t access Google fonts. I remember once being in this
  situation and doing everything possible to avoid reloading a project as
  I knew I’d lose the fonts and be forced to stop working.
- _Go beyond Google Fonts_. Some of my favorite typefaces aren’t on
  Google Fonts like [Clear Sans](https://01.org/clear-SANS), [Cooper
  Hewitt](https://www.cooperhewitt.org/open-source-at-cooper-hewitt/cooper-hewitt-the-typeface-by-chester-jenkins/),
  and
  [Aleo](https://www.behance.net/gallery/8018673/ALEO-Free-Font-Family).
- All web(site|app) dependencies should be managed through NPM whenever
  possible. Tis the modern way.

## What

Each typeface package ships with all the necessary font files and css to self-host an open source typeface.

## How

Couldn’t be easier. This is how you’d add Inter.

```shell
// with yarn
yarn add @typefaces-pack/typeface-inter

// with npm
npm install --save @typefaces-pack/typeface-inter
```

Then in your app or site’s entry file.

```shell
require('typeface-inter')

// or

import 'typeface-inter'
```

And that’s it! You’re now self-hosting of font Inter!

@typefaces-pack assumes you’re using webpack with loaders setup for loading css and font files (you can use Typeface with other setups but webpack makes things really really simple). Assuming your webpack configuration is setup correctly you then just need to require the typeface in the entry file for your project.

Many tools built with webpack such as [Gatsby](https://github.com/gatsbyjs/gatsby) and [Create React](https://github.com/facebook/create-react-app) App are already setup to work with Typefaces. Gatsby by default also embeds your CSS in your <head> for even faster loading.

If you’re not using webpack or equivalent tool that allows you to require css, then you’ll need to manually integrate the index.css and font files from the package into your build system.

## Whats Next

I could take the sources to the [project](https://github.com/KyleAMathews/typefaces) where I was inspired
