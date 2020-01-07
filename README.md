# Jekyll theme for GCweb
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v1.4%20adopted-ff69b4.svg)](code-of-conduct.md) [![Build Status](https://travis-ci.org/wet-boew/gcweb-jekyll.svg?branch=master)](https://travis-ci.org/wet-boew/gcweb-jekyll) [![Gem Version](https://badge.fury.io/rb/jekyll-theme-gcweb.svg)](https://badge.fury.io/rb/jekyll-theme-gcweb)

*GCweb is a Jekyll theme for Government of Canada websites. You can [preview the theme to see what it looks like](http://wet-boew.github.io/gcweb-jekyll), or even [use it today](#usage).*

## Usage

> **_NOTE:_** GCweb is the default theme for Government of Canada websites, but you can still specify the theme you're using as below.

To use the GCweb theme:

1. Add the following to your site's `_config.yml`:

    ```yml
    theme: jekyll-theme-gcweb
    ```

2. Optionally, if you'd like to preview your site on your computer, add the following to your site's `Gemfile`:

    ```ruby
    gem "github-pages", group: :jekyll_plugins
    ```



## Customizing

### Configuration variables

GCweb will respect the following variables, if set in your site's `_config.yml`:

```yml
title: [The title of your site]
description: [A short description of your site's purpose]
```

Additionally, you may choose to set the following optional variables:

```yml
google_analytics: [Your Google Analytics tracking ID]
```

### Stylesheet

If you'd like to add your own custom styles:

1. Create a file called `/assets/css/style.scss` in your site
2. Add the following content to the top of the file, exactly as shown:
    ```scss
    ---
    ---

    @import "{{ site.theme }}";
    ```
3. Add any custom CSS (or Sass, including imports) you'd like immediately after the `@import` line

### Layouts

If you'd like to change the theme's HTML layout:

1. [Copy the original template](https://github.com/wet-boew/gcweb-jekyll/blob/master/_layouts/default.html) from the theme's repository<br />(*Pro-tip: click "raw" to make copying easier*)
2. Create a file called `/_layouts/default.html` in your site
3. Paste the default layout content copied in the first step
4. Customize the layout as you'd like

## Roadmap

See the [open issues](https://github.com/wet-boew/gcweb-jekyll/issues) for a list of proposed features (and known issues).

## Project philosophy

The GCweb theme is intended to make it quick and easy for Government of Canada employees to create their first (or 100th) website of GitHub for their organisation. The theme should meet the vast majority of users' needs out of the box, erring on the side of simplicity rather than flexibility, and provide users the opportunity to opt-in to additional complexity if they have specific needs or wish to further customize their experience (such as adding custom CSS or modifying the default layout). It should also look great, but that goes without saying.

## How to Contribute

See [CONTRIBUTING.md](CONTRIBUTING.md)

------
_(French version will be available shortly)_

# Le thème Jekyll de GCweb
[![Build Status](https://travis-ci.org/wet-boew/gcweb-jekyll.svg?branch=master)](https://travis-ci.org/wet-boew/gcweb-jekyll) [![Gem Version](https://badge.fury.io/rb/jekyll-theme-gcweb.svg)](https://badge.fury.io/rb/jekyll-theme-gcweb)

*gcweb-jeckyll est un the Jekyll pour les sites web du gouvernement du Canada. Vous pouvez [voir un aperçu du thème pour avoir une idée de ce à quoi cela ressemble](http://wet-boew.github.io/gcweb-jekyll), ou sinon [vous pouvez l'utiliser maintenant](#utlisitation).*

## Utilisation

> **_REMARQUE :_** GCweb is the default theme for Government of Canada websites, but you can still specify the theme you're using as below.

To use the GCweb theme:

1. Add the following to your site's `_config.yml`:

    ```yml
    theme: jekyll-theme-gcweb
    ```

2. Optionally, if you'd like to preview your site on your computer, add the following to your site's `Gemfile`:

    ```ruby
    gem "github-pages", group: :jekyll_plugins
    ```



## Customizing

### Configuration variables

GCweb will respect the following variables, if set in your site's `_config.yml`:

```yml
title: [The title of your site]
description: [A short description of your site's purpose]
```

Additionally, you may choose to set the following optional variables:

```yml
google_analytics: [Your Google Analytics tracking ID]
```

### Stylesheet

If you'd like to add your own custom styles:

1. Create a file called `/assets/css/style.scss` in your site
2. Add the following content to the top of the file, exactly as shown:
    ```scss
    ---
    ---

    @import "{{ site.theme }}";
    ```
3. Add any custom CSS (or Sass, including imports) you'd like immediately after the `@import` line

### Layouts

If you'd like to change the theme's HTML layout:

1. [Copy the original template](https://github.com/wet-boew/gcweb-jekyll/blob/master/_layouts/default.html) from the theme's repository<br />(*Pro-tip: click "raw" to make copying easier*)
2. Create a file called `/_layouts/default.html` in your site
3. Paste the default layout content copied in the first step
4. Customize the layout as you'd like

## Roadmap

See the [open issues](https://github.com/wet-boew/gcweb-jekyll/issues) for a list of proposed features (and known issues).

## Project philosophy

The GCweb theme is intended to make it quick and easy for Government of Canada employees to create their first (or 100th) website of GitHub for their organisation. The theme should meet the vast majority of users' needs out of the box, erring on the side of simplicity rather than flexibility, and provide users the opportunity to opt-in to additional complexity if they have specific needs or wish to further customize their experience (such as adding custom CSS or modifying the default layout). It should also look great, but that goes without saying.

## Comment contribuer

Voir [CONTRIBUTING.md](CONTRIBUTING.md)