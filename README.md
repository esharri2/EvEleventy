# EvEleventy - An Eleventy Starter

This is an Eleventy starter project. It was made for me, Evan, but you might find it handy too. It uses Liquid templates, 
TailwindCSS, and PostCSS and Rollup.js for bundling.

## Features

### Commands

To start in development/watch mode: `npm start`. *Note that CSS is not watched*. You can run `npm run dev:css` to build the CSS.

Build: `npm run build`

### CSS

This starter uses [TailwindCSS](https://tailwindcss.com/). The CSS file is
generated by the PostCSS CLI tool. 

The Tailwind config has some basic customizations I like to use in projects, like a custom sizing system and Material-style shadows.

### Dark mode

Uses dark mode based on `prefers-color-scheme` (does not manually toggle.)

### Fonts

Fonts are included in `/fonts`. Fonts load via
["Unceremonious @font-face"](https://www.zachleat.com/web/comprehensive-webfonts/#font-face)
and the "display" font is
[preloaded](https://www.zachleat.com/web/comprehensive-webfonts/#preload) to
reduce [FOUT](https://www.zachleat.com/web/webfont-glossary/#fout).

### Icons

`_includes` contains the (Dripicons)[http://demo.amitjakhu.com/dripicons/] icon set. I'm using (
eleventy-plugin-svg-contents)[https://github.com/brob/eleventy-plugin-svg-contents] to easily render the icons inline. 

### Images

[eleventy-image](https://github.com/11ty/eleventy-img) generates multiple sizes of jpeg, webp, and avif for everything in `/images`. Use the `picture` shortcode to create a `<picture>` element that serves up the right image format based on browser support.

### JavaScript

Rollup.js is used to bundle everything in /scripts. 

### Navigation

Set up the site navigation in `_data/navigation.json` and footer navigation in `_data/navigation_footer.json`

### Pages

Pages includes a blog page with pagination already set up.

### Partials

`_includes` contains partials for some common components and elements.

### Production optimization

HTML, CSS, and JS minification happens during a production build.

