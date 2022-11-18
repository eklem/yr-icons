# Yr-icons

Icon set for weather data provided by [Yr.no](https://api.met.no/weatherapi/locationforecast/2.0/). Developed for monochrome e-paper/e-ink screens in mind. Heavily inspired by [Matmonsen/yr-icons](https://github.com/Matmonsen/yr-icons/). Used to be a fork.

[More information about the different weather symbols](https://hjelp.yr.no/hc/no/articles/203786121-V%C3%A6rsymbolene-p%C3%A5-Yr-) and [wind arrows](https://hjelp.yr.no/hc/no/articles/360002022134-Vindpiler-og-Beaufortskalaen). [Warning icons](https://hjelp.yr.no/hc/no/articles/360014052634-Farevarselikonene-p%C3%A5-Yr) may be developed later. [Create an issue](https://github.com/eklem/yr-icons/issues/new/choose) if there is something additional you need.

## Installation
Install from NPM
```console
npm i yr-icons
```

Reference the main css file
```html
  <link rel="stylesheet" href="./yr-icons/style.css">
```

CDN
```html
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/yr-icons@1.1.0/style.css">
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
  <i class="yr-wind-beauf-2 yr-wind-from-direction-10"></i>
  <i class="yr-wind-beauf-3 yr-wind-from-direction-20"></i>
  <i class="yr-wind-beauf-3 yr-wind-from-direction-30"></i>
```

## Icons
![Icons overview](https://raw.githubusercontent.com/eklem/yr-icons/trunk/icons-overview.png)

[HTML example for all weather and wind icons and css classes](https://eklem.github.io/yr-icons/example.html).

[License](https://github.com/eklem/yr-icons/blob/trunk/LICENSE)
