---
altLangPage: /fr/traductions
breadcrumbs:
  - title: "GCWeb Jekyll"
    link: "/en/index"
dateModified: 2021-06-31
description:
title: Translations
---
## Translations
In order to translate texts throughout the theme, modify the i18n-core.liquid file in the '_includes' folder and add the settings below.

```
%- elsif i18nText-lang == "en" -%\

  % assign i18nText-skipCont = "Skip to main content" %
  % assign i18nText-skipAbout = "Skip to About this site" %
  % assign i18nText-skipSection = "Skip to section menu" %

  % assign i18nText-altLang = "fr" %
  % assign i18nText-altLanguage = "Français" %

  % assign i18nText-search = "Search" %

  % assign i18nText-breadcrumb = "You are here:" %
  % assign i18nText-language = "Language selection" %

  % assign i18nText-menu = "Menu" %
  % assign i18nText-menuBtn = '<span class="wb-inv">Main </span>Menu' %

  % assign i18nText-signOnOff = "Sign-on information" %
  % assign i18nText-signOnRegister = "Register" %
  % assign i18nText-signIn = "Sign in" %
  % assign i18nText-signAs = "Signed in as" %
  % assign i18nText-signOut = "Sign out" %
  % assign i18nText-signAccount = "My account" %

  % assign i18nText-footerSite = "About this site" %
  % assign i18nText-top = "Top of Page" %

  % assign i18nText-dateModified = "Date modified:" %
```