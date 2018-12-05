# Colors

[![Open Source Love](https://badges.frapsoft.com/os/mit/mit.svg?v=102)](https://github.com/ellerbrock/open-source-badge/)
[![npm version](https://badge.fury.io/js/%40torq-design%2Fcolors.svg)](https://badge.fury.io/js/%40torq-design%2Fcolors)

This package defines a set of SCSS variables for the Torq Design color pallete.


<!-- #### [Demo in StackBlitz](https://stackblitz.com/edit/torq-typography-demo) -->

<!-- #### [Full Documentation](torqwebsite) -->


## Setup

#### Installation
Install the colors component in your project using npm.

```bash
npm i @torq-design/colors
```

#### Import SCSS

Import the SCSS file into your base styling file.

```css
@import "@torq-design/colors/torq-colors";
```

Make sure your project's SASS compiler is configured to look in the node_modules directory.


## Dark UI
| Variable                            | Uses                                 | Value     |
| :---------------------------------  | :----------------------------------  | :-------  |
| `$torq-primary-color`               | Calls to action, items of importance | `#508BE4` |
| `$torq-dark-background-top`         | Start to dark background gradient    | `#1A2633` |
| `$torq-dark-background-bottom`      | End to dark background gradient      | `#101820` |
| `$torq-dark-background`             | Dark page background                 | `linear-gradient(185.86deg, #1A2633 0%, #101820 100%)` |
| `$torq-dark-title-bar-background`   | Title bar background                 | `#151E26` |
| `$torq-dark-top-bar-background`     | Top bar background                   | `#1D2E40` |
| `$torq-dark-card-background`        | Card background                      | `#1D2E40` |
| `$torq-dark-outline`                | Outlines, table borders              | `#66757F` |
| `$torq-dark-text-color`             | General purpose text                 | `#FFFFFF` |
| `$torq-dark-header-text-color`      | Header text                          | `#FFFFFF` |
| `$torq-dark-subtext-color`          | Sub-text                             | `#A8B5BF` |
| `$torq-dark-chart-text-color`       | Chart text                           | `#A8B5BF` |


## Light UI
| Variable                            | Uses                                 | Value     |
| :---------------------------------  | :----------------------------------  | :-------  |
| `$torq-primary-color`               | Calls to action, items of importance | `#508BE4` |
| `$torq-light-background-top`        | Start to dark background gradient    | `#F7F9FB` |
| `$torq-light-background-bottom`     | End to dark background gradient      | `#D6DFEC` |
| `$torq-light-background`            | Dark page background                 | `linear-gradient(176.98deg, #F7F9FB 0%, #D6DFEC 100%)` |
| `$torq-light-title-bar-background`  | Title bar background                 | `#FFFFFF` |
| `$torq-light-top-bar-background`    | Top bar background                   | `#F7F7FB` |
| `$torq-light-card-background`       | Card background                      | `#FFFFFF` |
| `$torq-light-outline`               | Outlines, table borders              | `#C7D4DD` |
| `$torq-light-text-color`            | General purpose text                 | `#2C404C` |
| `$torq-light-header-text-color`     | Header text                          | `#202028` |
| `$torq-light-subtext-color`         | Sub-text                             | `#596578` |
| `$torq-light-chart-text-color`      | Chart text                           | `#596578` |

## Supporting Colors

Supporting colors are the same for both dark and light UI.

### Status

| Variable                            | Value     |
| :---------------------------------  | :-------  |
| `$torq-status-red`                  | `#F34336`   |
| `$torq-status-orange`               | `#FF8B3A`   |
| `$torq-status-yellow`               | `#FEC600`   |
| `$torq-status-green`                | `#7FAE1B`  |
| `$torq-status-blue`                 | `#508BE4`   |

### Data Visualization

| Variable                            | Value       |
| :---------------------------------  | :---------  |
| `$torq-data-pink`                   | `#F97DD8`   |
| `$torq-data-purple`                 | `#9150E4`   |
| `$torq-data-cyan`                   | `#50CCE4`   |
| `$torq-data-green`                  | `#61D883`   |
| `$torq-data-yellow`                 | `#E4CB50`   |
| `$torq-data-orange`                 | `#E4A350`   |