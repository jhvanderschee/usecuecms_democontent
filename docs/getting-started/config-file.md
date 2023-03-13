---
title: Config file setup
weight: 1
---

Here you will find the settings for a typical `config.yaml` file.

## Website URL

The most important thing is to set your domain name in the `baseURL`. This makes sure the right canonical URL will be displayed in your head. Additionally we advice you to use the `cononifyURLs` option. This allows you to publish your website on a different path (i.e. '/blog/') by adjusting just the `baseURL` (without the need to change all internal URL's).

```
baseURL: https://www.usecue.com
canonifyURLs: true
```
## Image resizing

To make sure all images can be resized we set the 'static' directory as the `assetDir`. This means that all static files will be part of Hugo's `resources` variable, thus can be resized.

```
assetDir: static
```

## Handling dates

You can define the order in which Hugo looks for a date. The following code instructs Hugo to look for the date in the filename first. If the filename does not start with a date, Hugo will look in the frontmatter for a variable called `date`. We advice you to put the date in the frontmatter, and not in the filename.

```
frontmatter:
  date:
    - :filename
    - date
```

## Setting the locale

Dates can be auto-formattted based on your language. It requires to correctly set your `languageCode` or your `defaultContentLanguage`.

```
languageCode: nl_NL
defaultContentLanguage: nl
```

## Multilingual setup

One of the great things in Hugo is the build in support for multilingual websites. Setting them up is done with the `languages` variable, as you can see below.

```
languages:
  en:
    languageName: English
    title: Usecue web development
    params: 
      description: Website development and web hosting
    contentDir: content/en
    weight: 1
    permalinks:
      posts: /blog/:slug
      portfolios: /portfolio/:slug
  nl:
    languageName: Nederlands
    title: Usecue web development
    params: 
      description: Website development en web hosting
    contentDir: content/nl
    weight: 2
    permalinks:
      posts: /blog/:slug
      portfolios: /portfolio/:slug
```
