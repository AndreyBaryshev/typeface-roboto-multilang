
# typeface-roboto

The CSS and web font files to easily self-host “Roboto”.

## Install

`npm install --save typeface-roboto`

## Use

Typefaces assume you’re using webpack to process CSS and files. Each typeface
package includes all necessary font files (woff2, woff, eot, ttf, svg) and
a CSS file with font-face declarations pointing at these files.

You will need to have webpack setup to load css and font files. Many tools built
with Webpack will work out of the box with Typefaces such as [Gatsby](https://github.com/gatsbyjs/gatsby)
and [Create React App](https://github.com/facebookincubator/create-react-app).

To use, simply require the package in your project’s entry file e.g.

```javascript
// Load Roboto typeface
require('typeface-roboto')
```

By default only basic subset of characters is included in the font file (it's Latin in most cases).
To add another one along the default, import specific CSS file.

```javascript
// Load Roboto typeface with Latin plus Latin Extended subset
require('typeface-roboto/latin-ext.css')

// Default subset is Latin
require('typeface-roboto/latin.css') === require('typeface-roboto')
```

## About the Typefaces project.

Our goal is to add all open source fonts to NPM to simplify using great fonts in
our web projects. We’re currently maintaining 865 typeface packages
including all typefaces on Google Fonts.

If your favorite typeface isn’t published yet, [let us know](https://github.com/KyleAMathews/typefaces)
and we’ll add it!
