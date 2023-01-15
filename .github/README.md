# Web site for greviegolf.se

The site is built using Jekyll and runs on GitHub Pages.

## Running Jekyll locally

Install `rbenv` to manage having multiple versions of Ruby installed on the machine.

Install Ruby 2.7.4 because GitHub Pages requires it:  https://pages.github.com/versions/

```
rbenv install 2.7.4
```

Use that version in the current dir:

```
rbenv local 2.7.4
```

Install Bundler:

```
gem install bundler:2.3.6
```

Run Jekyll:

```
bundle exec jekyll serve
```

Workaround hack to run GitHub pages with Ruby 3 and Python 3:

```
bundler exec jekyll build && bash -c 'cd _site && python3 -m http.server 3000'
```

## CSS

Overrides for CSS are in `assets/css/style.scss`

The generated CSS is in `_site/assets/css/style.css`

## Carousel

I've forgotten where I took the carousel code from, but it can be found in `_includes/carousel.html`

## Menu

The menu is controlled by `_data/docs.yml`

## Pages

The pages are in the root of the repository.
