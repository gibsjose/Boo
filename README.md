# Boo
###### *A fresh Ghost theme.*

## Description
Boo is based off of [Casper](https://github.com/TryGhost/Casper), the default theme for [Ghost](http://github.com/tryghost/ghost/).

For a **detailed** look at how I created this theme, with tons of code samples and instructions, see my blog post on [Ghost Themes](http://microamps.gibsjose.com/ghost-themes). There are also other posts there about setting up a host (through DigitalOcean) for your blog, and adding security to your site with CloudFlare, among other things.

## Installation
To install this theme, clone it into your `ghost` themes directory (usually `/var/www/ghost/content/themes`), then restart `ghost` with `sudo service ghost restart`.

On Ubuntu:
```bash
export GHOST_DIR='/var/www/ghost' # Modify this to your Ghost directory
cd $GHOST_DIR/content/themes

# Clone it here...
git clone git@github.com/gibsjose/Boo.git

# Restart Ghost
sudo service ghost restart
```

## Customization
To get the most out of this theme, you will have to customize a few things:

#### 1. Small Post Logos
The small logo displayed on each post in the upper left corner is separate from the Blog logo you uploaded on your Ghost admin page.

To use your own logo, simply replace `assets/img/post-logo.png` and `assets/img/post-logo-hover.png` with your own artwork.

#### 2. `favicon`
To use your own icon as the `favicon`, the little icon displayed on tabs and for bookmarks in your browser, simply replace `assets/favicon.ico` with your own artwork.

#### 3. Disqus Comments
To link the Disqus comments to your own account (you will need an account if you don't have one already), you will need to use your own username in both `post.hbs` and `default.hbs`.

Change `username` in
```javascript
var disqus_shortname = 'username';
```
to your own Disqus username.

#### 4. Author Metadata
Unless you want people on your blog being linked to my GitHub and Twitter accounts (I'd be very flattered), you should change the links contained in `post.hbs` under the `author` section.
