# Web site for greviegolf.se

The site is built using Jekyll and runs on GitHub Pages.

## Running Jekyll locally

Because I am running Python 3 and Ruby 3 (too new), I have to do a bit of a hack to run the site locally: 

```
bundler exec jekyll build && bash -c 'cd _site && python3 -m http.server 3000'
```

...instead of the simpler:

```
bundle exec jekyll serve
```

GitHub Pages currently requires Ruby 2.7.4 but maybe one day it will work with Ruby 3.
See: https://pages.github.com/versions/

## CSS

Overrides for CSS are in `assets/css/style.scss`

The generated CSS is in `_site/assets/css/style.css`

## Carousel

I've forgotten where I took the carousel code from, but it can be found in `_includes/carousel.html`

## Menu

The menu is controlled by `_data/docs.yml`

## Pages

The pages are in the root of the repository.
