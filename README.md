# Boo
###### *A fresh Ghost theme.*

## Description
Boo is based off of [Casper](https://github.com/TryGhost/Casper), the default theme for [Ghost](http://github.com/tryghost/ghost/).

For a **detailed** look at how I created this theme, with tons of code samples and instructions, see my blog post on [Ghost Themes](http://microamps.gibsjose.com/ghost-themes)

## Installation
To install this theme, download the latest release zip/tarball into your `ghost` themes directory and extract it, then restart `ghost`.

On Ubuntu:
```bash
export GHOST_DIR='/var/www/ghost' # Modify this to your Ghost directory
cd $GHOST_DIR/content/themes

# Extract archive here...

sudo service ghost restart
```

## Customization
To get the most out of this theme, you will have to customize a few things:

#### 1. Small Post Logos
The small logo displayed on each post in the upper left corner is separate from the Blog logo you uploaded on your Ghost admin page.

To use your own logo, simply replace `assets/img/post-logo.png` and `assets/img/post-logo-hover.png` with your own artwork.

#### 2. `favicon`
To use your own icon as the `favicon`, the little icon displayed on tabs and for bookmarks in your browser, simply replace `assets/favicon.ico` with your own artwork.

#### 2. Disqus Comments
To link the Disqus comments to your own account (you will need an account if you don't have one already), you will need to use your own username in both `post.hbs` and `default.hbs`.

Change `username` in
```javascript
var disqus_shortname = 'username';
```
to your own Disqus username.
