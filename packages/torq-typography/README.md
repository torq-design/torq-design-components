# Typography

[![Open Source Love](https://badges.frapsoft.com/os/mit/mit.svg?v=102)](https://github.com/ellerbrock/open-source-badge/)
[![npm version](https://badge.fury.io/js/%40torq-design%2Ftypography.svg)](https://badge.fury.io/js/%40torq-design%2Ftypography)

This package imports Heebo (the chosen font for Torq Design) and sets it as the default font.  It also defines a set of font profiles and the default sizes, weights, etc. for those profiles.

#### Font Profiles

| SCALE CATEGORY | HTML TAG                    | CSS CLASS                    | USAGE               | FONT    | SIZE | TRACKING | LINE HEIGHT |
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


#### Available font weights

| Weight     | Value | CSS Class             |
| :--------: | :---: | :-------------------: |
| Light      | 300   | `weight--light`       |
| Regular    | 400   | `weight--regular`     |
| Medium     | 500   | `weight--medium`      |
| Bold       | 700   | `weight--bold`        |
| Extra Bold | 800   | `weight--extra-bold`  |


## Installation
Install the typography component in your project using npm.

```npm i @torq-design/typography```

## Usage

Import the SCSS file into your base styling file.

```@import "@torq-design/typography/torq-typography";```

Make sure your project's SASS compiler is configured to look in the node_modules directory.

#### HTML Tag Defaults

Using any of the HTML tags listed in the table above will automatically apply the corresponding font characteristics.

```<h4>This is a section header</h4>```

#### Font Profile Classes

This can also be achieved through the use of the CSS classes.

```<div class="torq-typ--section-header">This is also a section header.</div>```

#### Font Weight Classes

Adjust font weights using the available CSS classes.

```<div class="weight--extra-bold">This is some extra bold text.</div>```