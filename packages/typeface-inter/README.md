<div align="center">

# @typefaces-pack/typeface-inter

The CSS and web font files to easily self-host [inter](https://rsms.me/inter/).

  <a href="https://www.npmjs.com/package/@typefaces-pack/typeface-inter" target="_blank">
    <img src="https://img.shields.io/npm/v/@typefaces-pack/typeface-inter?color=red&style=flat-square" alt="www.npmjs.com" />
  </a>

</div>

## Install

```shell
// with yarn
yarn add @typefaces-pack/typeface-inter

// with npm
npm install --save @typefaces-pack/typeface-inter
```

## Use

`@typefaces-pack` assume you’re using webpack to process CSS and files. Each typeface
package includes all necessary font files (woff2, woff) and a CSS file with
font-face declarations pointing at these files.

You will need to have webpack setup to load css and font files. Many tools built
with Webpack will work out of the box with Typefaces such as [Gatsby](https://github.com/gatsbyjs/gatsby)
and [Create React App](https://github.com/facebookincubator/create-react-app).

To use, simply require the package in your project’s entry file e.g.

```shell
require('typeface-inter')

// or

import 'typeface-inter'
```
