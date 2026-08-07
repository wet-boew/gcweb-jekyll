---
altLangPage: /en/setup
breadcrumbs:
  - title: "GCWeb Jekyll"
    link: "/fr/index"
dateModified: 2021-06-31
description:
title: Configuration
---

## Environment

Avant de commencer, assurez-vous d'avoir [Ruby](https://www.ruby-lang.org/en/documentation/installation/) et [NodeJS](https://nodejs.org/) d'installer.

Puis installer Jekyll:

```
$ gem install jekyll
```

## Installer le gabarit

1. Créez un dépôt pour votre projet :

```
$ git init https://github.com/<votre-nom-d-usager-github>/<nom-du-projet>
```

2. Accéder à votre projet localement :

```
$ cd chemin/daccess/au/nom-du-projet
```

3. Exécuter Jekyll:

```
$ bundle exec jekyll build
```

## Rouler localement

Après les étapes ci-dessus, pour exécuter Jekyll localement, ...:

```
$ bundle exec jekyll serve
```

## Personnalisation

Le gabarit GCWeb-Jekyll vous permet de personnaliser votre site avec plusieurs paramètres. Lisez la [documentation](personnalisation.html) pour plus de détails.

Pour une personnalisation avancée du thème, consultez le [dépôt GCWeb](https://github.com/wet-boew/GCWeb) pour les fichiers de style.