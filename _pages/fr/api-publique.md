---
title: L'API publique du thème du gcweb-jekyll
---

## Liste des changements

* Nom des fichier _includes et _layouts
* Le scope de chacun des fichier _includes et _layouts ainsi que leur but.
  * Example -> fichier: gcweb-menu/inc-sitemenu.html scope: "dans le header" but: "Menu"

* La liste des paramètres dans le front-matter
  * title
  * altLangPage
  
* Les variable Liquid pour i18n et global du thème
* Liste des variables du site (_config.yml) considéré pour les setting du thème. Tel qu'utilisé dans : variable-core.liquid

* i18n.liquid -> Spécifique au thème de Canada.ca, Leur override peut permettre la création de sous thème.
  * i18nText-sigBlk
	* i18nText-goc
	* i18nText-gocAltLang
  * i18nText-searchSite
	* i18nText-home
	* i18nText-menuAjax
	* i18nText-feedback
	* i18nText-footerAbout
	* i18nText-wmms
	* i18nText-wmmsAltLang

* i18n-core.liquid -> Texte générique et réutilisable au delas du thème. example "Passer au contenu principal" qui est utilisé pour le skip link.

* settings.liquid -> Paramètre du site, example "Base path" pour les bibliothèque javascript et CSS.
  * setting-resourcesBasePath
  * setting-resourcesBasePathWetboew
  * setting-packageName
  * setting-minifiedSuffix 


* Liste et emplacement des assets de GCWeb
  * FIP images
  * JS
  * CSS

----

## Bonne pratiques à documenté

* Utilisation des métadonnées obligatoire: 
  * Title
  * Creator
  * Language
  * Issued
  * Modified
  * Subject

---

## Dépendance du thème

* Conçu pour Jekyll v3 tel supporté par Github pages

