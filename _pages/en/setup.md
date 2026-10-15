---
altLangPage: /fr/configuration
breadcrumbs:
  - title: "GCWeb Jekyll"
    link: "/en/index"
dateModified: 2021-06-31
description:
title: Setup
---
## Environment
Before starting, make sure you have [Ruby](https://www.ruby-lang.org/en/documentation/installation/) and [NodeJS](https://nodejs.org/) installed.

Then install Jekyll:
```
$ gem install jekyll
```

## Installing the template

1. Create a repo for your project:
```
$ git init https://github.com/<your-github-username>/<your-project-name>
```

2. Access the local project:
```
$ cd path/to/your-project-name
```

3. Set the _config.yml to call the gcweb-jekyll theme

```
remote_theme: wet-boew/gcweb-jekyll
```

4. Build Jekyll:
```
$ bundle exec jekyll build
```

## Running local
After the steps above, to run Jekyll locally, ...:
```
$ bundle exec jekyll serve
```

## Customization
Jekflix Template allows you to personalize your site with several settings. Read the [docs](settings.html) for more details.

For advanced theme customization, check the [GCWeb repo](https://github.com/wet-boew/GCWeb) for style files.