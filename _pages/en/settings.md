---
altLangPage: /fr/personnalisation
breadcrumbs:
  - title: GCWeb Jekyll
    link: /en/index
dateModified: 2021-06-31
description:
title: Settings
---
Customize your website layout, titles and more. The settings file can be found in `_config.yml`.

## Site settings

The general settings have to be set in `_config.yml`.

> **Important**: The minimum requirement to configure your website, would be to set the `remote_theme: WET-BOEW/gcweb-jekyll` in your config file

### `site-description`

Type: *dictionary*

The website description is used for SEO purposes only.

Example:

```yml
# _config.yml

site-description:
  en: A reference implementation of the Canada.ca Content and Information Architecture Specification, the Canada.ca Content Style Guide and the Canada.ca Design System.
  fr: "Une mise en œuvre de référence de la spécification de l'architecture du contenu et de l'information de Canada.ca, du guide de style de contenu de Canada.ca et du système de conception de Canada.ca."
```

### `title`

Type: *string*

The website title is used for SEO purposes and set the home page title.

Example:

```yml
# _config.yml

title: GCWeb Jekyll | A remote Jekyll theme with the Canada.ca theme.
```


## Page settings

The page settings have to be set in the Front Matter of the page content

> **Important**: Some settings could be set as default in the `_config.yml` file

### `altLangPage`

Type: *string*

The altLangPage file path is used to enable the link in the language toggle for the translation of the alternate page content. If omitted, the link in the language won't be added in the header.

Example:

```yml
# page.md

---
altLangPage: /fr/page
---
```

### `breadcrumbs`

Type: *array*

The breadcrumbs items are used to enable the links in the breadcrumbs. A title and an absolute url for each breadcrumb is required.

Example:
```yml
# page.md

---
breadcrumbs:
  - title: Canada.ca
    link: https://www.canada.ca/en
---
```

### `css`

Type: *string* or *array*

The css file path is used to attach custom stylesheets to your page. If you have more than one stylesheets to attach use the array format to declare them, otherwise the string format can be used if you only have one stylesheet to attach.

Example:
```yml
# page.md

---
css:
  - /path/to/stylesheet1
  - /path/to/stylesheet2
  - ...
---
```

### `dateModified`

Type: *date*

The date is used to specified the last modification date of the page in ISO format, AAAA-MM-DD.

Example:

```yml
# page.md

---
dateModified: 2021-07-01
---
```

## `description`

Type: *string*

The page description is used for SEO purpose only. As its value cannot be zero, if it is not defined in the page, the site description will be used instead.

Example:

```yml
# page.md

---
description: Page description for SEO
---
```

### `lang`

Type: *string*

The lang property is used to specifiy the language of the page content. By default the template support "en" for English and "fr" for French.

Example:

```yml
# page.md

---
lang: en
---
```

### `layout`

Type: _string_

The page layout is used to define the page template to use. There's eight templates that can be called from your page:

- *core**
- *default*
- *fluid*
- *layout-home*
- *layout-servermessage*
- *layout-splashpage*
- *no-container*
- *without-h1*

\* The core template should be used to create other templates.

Example:

```yml
# page.md

---
layout: default
---
```

### `nofooter`

Type: *bolean*

The nofooter setting is used to disable the global site footer when set to true. If the global site footer is disabled, the skiplinks will be adjusted accordingly.

Example:
```yml
# page.md

---
nofooter: true
---
```

### `pageclass`

Type: *string*

* splash
* page-type-nav
* cnt-wdth-lmtd
* page-type-search
* theme

Example:
```yml
# page.md

---
pageclass: cnt-wdth-lmtd
---
```

### `pageType`

Type: *string*

* advance service
* archived
* gcaudience
* institution
* news
* organization
* theme
* topic

Example:
```yml
# page.md

---
pageType: archived
---
```

### `script`

Type: *string* or *array*

The css file path is used to attach custom scripts to your page. If you have more than one script files to attach use the array format to declare them, otherwise the string format can be used if you only have one script file to attach.

Example:
```yml
# page.md

---
script:
  - /path/to/script1
  - /path/to/script2
  - ...
---
```

### `title`

Type: *string*

Example:
```yml
# page.md

---
title: Title of the website or webpage
---
```

### `titleH1`

Type: *string*

Example:
```yml
# page.md

---
titleH1: Text to override the title of the webpge in the H1
---
```

## `layout-splashpage` settings

### `creator-en`

Type: *string*

The creator-en is used for SEO purpose only and set the page creator English name.

```yml
# index.md

---
creator-en: Department name
layout: layout-splashpage
---
```

### `creator-fr`

Type: *string*

The creator-en is used for SEO purpose only and set the page creator French name.

Example:
```yml
# index.md

---
creator-fr: Nom du ministère
layout: layout-splashpage
---
```

### `dateIssued`

Type: *date*

Example:
```yml
# index.md

---
dateIssued: 2021-07-01
layout: layout-splashpage
---
```

### `description-en`

Type: *string*

Example:
```yml
# index.md

---
description-en: Page description for SEO
layout: layout-splashpage
---
```

### `description-fr`

Type: *string*

Example:
```yml
# index.md

---
description-fr: Description de la page pour fins de référencement
layout: layout-splashpage
---
```

### `subject-en`

Type: *string*

Example:
```yml
# index.md

---
subject-en: topic1, topic2, topic3, ...
layout: layout-splashpage
---
```

### `subject-fr`

Type: *string*

Examples:
```yml
# index.md

---
subject-fr: sujet1, sujet2, sujet3, ...
layout: layout-splashpage
---
```