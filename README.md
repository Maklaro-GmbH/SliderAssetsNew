# Static assets for Maklaro Slider

**IMPORTANT !!! Only edit or delete files if you really know what you are doing!**

## Deployments

There is only a `master` branch. Deployments there will automatically go to production on Netlify.

The deployment URL is: https://slider-assets.maklaro.com (Netlify domain: https://maklaro-slider-assets.netlify.app).

## SVG coloring

At the moment you can set two different classes that support coloring for the icons. One is `fill-gray` and the other `fill-primary`.

Depending on the UI, you want to have the whole icon in a grayscale or colored. But you could also have a combination of both.

Example with `year.svg`:

```html
<svg xmlns="http://www.w3.org/2000/svg" width="128" height="128" viewBox="0 0 128 128">
 <g>
  <polygon class="fill-primary" points="[...]"/>
  <polygon class="fill-primary" points="[...]"/>
  <path class="fill-gray" fill-rule="nonzero" d="[...]"/>
 </g>
</svg>
```

These colors are set dynamically in the Slider project, but you can overwrite the default colors with the config file.

Example configuration:

```json
[...]

colors: {
    iconFillPrimary: '#BAE0FD',
    iconFillGray: '#444444'
}

[...]
```
