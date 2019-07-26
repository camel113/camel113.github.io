# Adrien Bigler's blog

## Intro
This blog runs with [Jekyll](https://jekyllrb.com/) and is hosted with [Github pages](https://pages.github.com/). This is a very efficient way to make personnal blogs and simple small websites for free.

## Dev

To simplify development use [browsersync](https://www.browsersync.io) with this command `browser-sync start --proxy "localhost:4000" --files "_site/*.*"`

Sass dev mode: `sass --watch _assets/styles/main.scss assets/styles/main.css --no-source-map` (while running browsersync)

Sass prod mode: `sass  _assets/styles/main.scss _includes/main.css --no-source-map --style compressed`

_to_do_

Remplacer le process pour la minimisation CSS/SASS et l'implantation du CSS dans le html...

## Workflow to make website faster

### Post's image
Respect the ratio `480:250` and at least `width:480px` and `height:250px`. Recommanded dimmensions `width:960px` and `height:500px`.

### CSS Inine
Run `gulp sass:critical` to include critical CSS directly in html files.