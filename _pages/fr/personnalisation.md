---
altLangPage: /en/settings
breadcrumbs:
  - title: "GCWeb Jekyll"
    link: "/fr/index"
dateModified: 2021-06-31
description:
title: Personnalisation
---
Personnalisez la mise en page de votre site Web, les titres et plus encore. Les paramètres se trouvent dans le fichier `_config.yml`.

## Paramètres du site

Les paramètres généraux doivent être définis dans `_config.yml`.

> **Important** : La configuration minimale requise pour configurer votre site Web serait de définir le `remote_theme: WET-BOEW/gcweb-jekyll` dans votre fichier de configuration

### `site-description`

Type : *dictionaire*

La description du site Web est utilisée uniquement à des fins de référencement (SEO).

Exemple :

```yml
# _config.yml

site-description:
  en: A reference implementation of the Canada.ca Content and Information Architecture Specification, the Canada.ca Content Style Guide and the Canada.ca Design System.
  fr: "Une mise en œuvre de référence de la spécification de l'architecture du contenu et de l'information de Canada.ca, du guide de style de contenu de Canada.ca et du système de conception de Canada.ca."
```

### `title`

Type : *chaîne de caractères*

Le titre du site Web est utilisé à des fins de référencement (SEO) et définit le titre de la page d'accueil.

Exemple :

```yml
# _config.yml

title: GCWeb Jekyll | Un thème Jekyll à distance avec le thème Canada.ca.
```


## Paramètres de la page

Les paramètres de la page doivent être définis dans le Front Matter du contenu de la page

> **Important** : Certains de ces paramètres peuvent être définis par défaut dans le fichiers `_config.yml`.

### `altLangPage`

Type : *chaîne de caractères*

Le chemin du fichier altLangPage est utilisé pour activer le lien dans la bascule de langue pour la traduction du contenu de la page alternative. S'il est omis, le lien dans la langue ne sera pas ajouté dans l'en-tête.

Exemple :

```yml
# page.md

---
altLangPage: /fr/page
---
```

### `breadcrumbs`

Type: *tableau*

Les items dans la propriété breadcrumbs est utilisé pour activer les liens dans le fil d'Arianne. Un titre et un lien absolu est requis pour chaque item.

```yml
# page.md

---
breadcrumbs:
  - title: Canada.ca
    link: https://www.canada.ca/fr
---
```

### `css`

Type: *chaîne de caractères* ou *tableau*

Le chemin des fichiers css est utilisé pour ajouter des feuilles de style personalisées à votre page. Si vous avez plus d'une feuille à ajouter, utilisez un tableau pour les déclarer, sinon le format de chaìne de caractères peut être utilisé si il n'y a qu'une seule feuille de style à ajouter.

Example:
```yml
# page.md

---
css:
  - /chemin/du/fichier/de/la/feuile-de-style1
  - /chemin/du/fichier/de/la/feuile-de-style2
  - ...
---
```

### `dateModified`

Type : *date*

La date permet de préciser la date de dernière modification de la page au format ISO, AAAA-MM-JJ.

Exemple:

```yml
# page.md

---
dateModified: 2021-07-01
---
```

### `description`

Type : *chaîne de caractères*

La description de la page est est utilisée uniquement à des fins de référencement (SEO). Comme sa valeur ne peut être nulle, si elle n'est pas définie dans la page, la description du site sera utilsé.

```yml
# page.md

---
description: Description de la page pour fins de référencement
---
```

### `lang`

Type : *chaîne de caractères*

La propriété lang est utilisée pour spécifier la langue du contenu de la page. Par défaut, le modèle prend en charge "en" pour l'anglais et "fr" pour le français.

Exemple :

```yml
# page.md

---
lang: fr
---
```

### `layout`

Type : _chaîne de caractères_

La mise en page permet de définir le modèle de page à utiliser. Huit modèles peuvent être appelés à partir de votre page :

- *core*
- *default*
- *fluid*
- *layout-home*
- *layout-servermessage*
- *layout-splashpage*
- *no-container*
- *without-h1*

Exemple :

```yml
# page.md

---
layout: défault
---
```