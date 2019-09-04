# Typography

[![Open Source Love](https://badges.frapsoft.com/os/mit/mit.svg?v=102)](https://github.com/ellerbrock/open-source-badge/)
[![npm version](https://badge.fury.io/js/%40torq-design%2Ftypography.svg)](https://badge.fury.io/js/%40torq-design%2Ftypography)

This package defines a set of font profiles for Torq Design.


#### [Demo in StackBlitz](https://stackblitz.com/edit/torq-typography-demo)


## Setup

#### Installation
Install the typography component in your project using npm.

```bash
npm i @torq-design/typography
```

#### Import Sass

Import the Sass file into your base styling file.

```css
@import "@torq-design/typography/torq-typography";
```

Make sure your project's SASS compiler is configured to look in the node_modules directory.

#### Import CSS

We do offer a pre-compiled CSS version if your project doesn't use SCSS.

```html
<link rel="stylesheet" href="../../node_modules/@torq-design/typography/css/torq-typography.css">
```
Or 
```css
@import "../../node_modules/@torq-design/typography/css/torq-typography.css";
```

#### Import Font

Import our default font (Roboto) in your root HTML file.

```html
<link href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Roboto+Slab" rel="stylesheet">
```

Or, import the font in your base styling file.

```css
@import url('https://fonts.googleapis.com/css?family=Roboto:300,400,500,700');
@import url('https://fonts.googleapis.com/css?family=Roboto+Slab');
```

If you need weights beyond those used in our font profiles, feel free to customize the import [here.](https://fonts.google.com/specimen/Roboto?selection.family=Roboto:300,400,500,700)
You can also add the italic variants for different weights if that's necessary.

#### Apply Base Font
Use our base css class to make Roboto the default font.
```html
<body class="torq-typ">
```
Or, use the Sass mixin.
```scss
body {
  @include torq-typ-base;
}
```

## Font Profiles
| SCALE CATEGORY | HTML TAG                    | CSS CLASS                    | USAGE               | WEIGHT  |SIZE\*|TRACKING\*|LINE HEIGHT\*| TYPEFACE\*    | 
| :------------: | :-------------------------  | :--------------------------  | :-----------------  | :-----: | :--: | :------: | :---------: | :-----------: |
| H1             | `<h1>`                      | `torq-typ--h1`               | KPI's               | Any     | 50px | 0        | 73px        | Roboto        |
| H2             | `<h2>`                      | `torq-typ--h2`               | KPI's               | Any     | 38px | 0        | 56px        | Roboto        |
| H3             | `<h3>`                      | `torq-typ--page-header`      | Page Headers        | Regular | 24px | 0        | 35px        | Roboto        |
| H4             | `<h4>`                      | `torq-typ--section-header`   | Card Header         | Bold    | 20px | Auto     | 29px        | Roboto        |
| H5             | `<h5>`                      | `torq-typ--title1`           | Title 1             | Medium  | 18px | Auto     | 27px        | Roboto        |
| H6             | `<h6>`                      | `torq-typ--title2`           | Title 2             | Bold    | 15px | Auto     | 26px        | Roboto        |
| Body 1         | `<p>`, `<button>` | `torq-typ--body1`            | Body Copy & Buttons | Medium  | 15px | Auto     | 26px        | Roboto        |
| Body 2         | `<span>`, `<p>`, `<div>`    | `torq-typ--body2`            | Paragraph Text      | Regular | 15px | Auto     | 26px        | Roboto        |
| Charts         | `<table>`, `<th>`           | `torq-typ--chart-title`      | Chart Titles        | Medium  | 13px | 0.13px   | 15px        | Roboto        |
| Notes          | `<p>`, `<span>`, `<div>`    | `torq-typ--small-text`       | Small text          | Medium  | 13px | 0.13px   | 15px        | Roboto        |
| App name       | `<title>`                   | `torq-typ--branding`         | Branding            | Bold    | 15px | Auto     | 20px        | Roboto Slab   |



\*_Sizes are actually implemented using rem, assuming a base font size of 16px._

#### Tag Defaults

Using any of the HTML tags listed in the table above will automatically apply the corresponding font characteristics.

```html
<h4>This is a section header</h4>
```

#### Font Profile CSS Classes

Each font profile has an accompanying CSS class.

```html
<div class="torq-typ--section-header">This is also a section header.</div>
```

#### Sass Mixins

A Sass mixin can also be used to apply the various font profiles. Use the same names from the css classes.
```scss
.custom-section-header {
  @include torq-typ(section-header);
}
```

## Font Weights


| Weight     | Value | CSS Class             |
| :--------: | :---: | :-------------------: |
| Thin\*\*   | 100   | `weight--thin`        |
| Light      | 300   | `weight--light`       |
| Regular    | 400   | `weight--regular`     |
| Medium     | 500   | `weight--medium`      |
| Bold       | 700   | `weight--bold`        |
| Black\*\*  | 900   | `weight--black`       |

\*\*_Not normally used in Torq Design, but available in Roboto font with a customized import_

#### Adjust font weights using the available CSS classes.

```html
<div class="weight--bold">This is some bold text.</div>
```

## Acknowledgements
This component is a modified version of Google's Material Design for Web typography component.

* [Github](https://github.com/material-components/material-components-web/tree/master/packages/mdc-typography)
* [License (MIT)](https://github.com/material-components/material-components-web/blob/master/LICENSE)