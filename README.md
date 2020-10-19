# Yr-icons

Icon set for weather data provided by [Yr.no](https://hjelp.yr.no/hc/no/articles/360001940793-Gratis-v%C3%A6rdata-fra-Yr)
A fork of [Matmonsen/yr-icons](https://github.com/Matmonsen/yr-icons/blob/master/LICENSE). Forked to be able to create a NPM package and add a wind arrow font + css for those.

[More information about the different weather symbols](http://om.yr.no/forklaring/symbol/)

## Installation
Install from NPM
```console
npm i yr-icons
```

Reference the main css file
```html
  <link rel="stylesheet" href="./yr-icons/style.css">
```
## Usage
Yr's location forecast outputs weather summaries like `clearsky_day` or `lightssnowshowersandthunder_day`. The weather icons have matching CSS class references for easy integration. HTML example:
```html
  <i class="yr-icon-clearsky_day"></i>
  <i class="yr-icon-lightssnowshowersandthunder_day"></i>
  <i class="yr-icon-fog"></i>
```
The wind arrows follows the Beaufort scale, which needs a translation from meters/second that the same Yr API outputs. The good part is that wind direction is easily translated from Yr's API. The only thing you need to do is to round the number to the closest integer.

```html
  <i class="ico yr-wind-beauf-2 yr-wind-from-direction-10"></i>
  <i class="ico yr-wind-beauf-3 yr-wind-from-direction-20"></i>
  <i class="ico yr-wind-beauf-3 yr-wind-from-direction-30"></i>
```

[HTML example for all weather and wind icons and css classes](https://eklem.github.io/yr-icons/example.html).

## [License - Yr weather icons](https://github.com/eklem/yr-icons/blob/master/LICENSE-weather)
## [License - Yr wind beaufort scale icons](https://github.com/eklem/yr-icons/blob/master/LICENSE-wind)
