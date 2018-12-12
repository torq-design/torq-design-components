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

#### Import SCSS

Import the SCSS file into your base styling file.

```css
@import "@torq-design/typography/torq-typography";
```

Make sure your project's SASS compiler is configured to look in the node_modules directory.

#### Import CSS

We do offer a pre-compiled CSS version if your project doesn't use SCSS.

```html
<link rel="stylesheet" href="../../node_modules/@torq-design/typography/torq-typography.css">
```
Or 
```css
@import "../../node_modules/@torq-design/typography/torq-typography.css";
```

#### Import Font

Import our default font in your root HTML file.

```html
<link href="https://fonts.googleapis.com/css?family=Heebo:300,400,500,700,800" rel="stylesheet">
```

Or, import the font in your base styling file.

```css
@import url('https://fonts.googleapis.com/css?family=Heebo:300,400,500,700,800');
```

## Font Profiles
| SCALE CATEGORY | HTML TAG                    | CSS CLASS                    | USAGE               | WEIGHT  | SIZE | TRACKING | LINE HEIGHT |
| :------------: | :-------------------------  | :--------------------------  | :-----------------  | :-----: | :--: | :------: | :---------: |
| H1             | `<h1>`                      | `torq-typ--h1`               | Widgets             | Regular | 50px | Auto     | Auto        |
| H2             | `<h2>`                      | `torq-typ--h2`               | Widgets             | Regular | 38px | Auto     | Auto        |
| H3             | `<h3>`                      | `torq-typ--page-header`      | Page Headers        | Regular | 24px | 0        | 35px        |
| H4             | `<h4>`                      | `torq-typ--section-header`   | Section Header      | Bold    | 20px | Auto     | 29px        |
| H5             | `<h5>`                      | `torq-typ--title1`           | Title 1             | Bold    | 18px | Auto     | 27px        |
| H6             | `<h6>`                      | `torq-typ--title2`           | Title 2             | Bold    | 15px | Auto     | 26px        |
| Body 1         | `<body>`, `<p>`, `<button>` | `torq-typ--body1`            | Body Copy & Buttons | Medium  | 15px | 0        | 26px        |
| Body 2         |                             | `torq-typ--body2`            | Body Copy & Buttons | Light   | 15px | 0        | 26px        |
| Charts         |                             | `torq-typ--chart-title`      | Chart Titles        | Medium  | 13px | 0.13px   | 40px        |

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

#### SCSS Mixins

An SCSS mixin can also be used to apply the various font profiles. Use the same names from the css classes.
```scss
@import @torq-design/typography/mixins;

.custom-section-header {
  @include torq-typ(section-header);
}
```

## Font Weights

| Weight     | Value | CSS Class             |
| :--------: | :---: | :-------------------: |
| Light      | 300   | `weight--light`       |
| Regular    | 400   | `weight--regular`     |
| Medium     | 500   | `weight--medium`      |
| Bold       | 700   | `weight--bold`        |
| Extra Bold | 800   | `weight--extra-bold`  |

Adjust font weights using the available CSS classes.

```html
<div class="weight--extra-bold">This is some extra bold text.</div>
```

## Acknowledgements
This component is a modified version of Google's Material Design for Web typography component.

* [Github](https://github.com/material-components/material-components-web/tree/master/packages/mdc-typography)
* [License (MIT)](https://github.com/material-components/material-components-web/blob/master/LICENSE)