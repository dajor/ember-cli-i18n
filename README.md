# Easy i18n

[![Build](https://travis-ci.org/dockyard/easy-i18n.svg?branch=master)](https://travis-ci.org/dockyard/easy-i18n)

## About ##

Simple Internationalization support for ember-cli apps.

## Install ##

```bash
npm install easy-i18n --save-dev
```

## Usage ##

### Translate

#### Configuration

In your app's `config/environment.js` you'll need to set
`ENV.APP.defaultLocale` to a country code:

```javascript
var ENV = {
  APP: {
    defaultLocale: 'en'
  }
};
```

#### Locale Files

Generate a new locale file:

```
ember g locale en
```

The file will be added to `app/locales'

```
app/
└── locales
    └── en.js
```

The content export a single POJO:

```javascript
export default {
  home: {
    title: 'Welcome'
  }
};
```

#### Helper

You can access the translations in your app with the `t` helper:

```handlebars
{{t 'home.title'}}
```

## Authors ##

* [Brian Cardarella](http://twitter.com/bcardarella)

[We are very thankful for the many contributors](https://github.com/dockyard/easy-i18n/graphs/contributors)

## Versioning ##

This library follows [Semantic Versioning](http://semver.org)

## Want to help? ##

Please do! We are always looking to improve this gem. Please see our
[Contribution Guidelines](https://github.com/dockyard/easy-i18n/blob/master/CONTRIBUTING.md)
on how to properly submit issues and pull requests.

## Legal ##

[DockYard](http://dockyard.com), Inc &copy; 2014

[@dockyard](http://twitter.com/dockyard)

[Licensed under the MIT license](http://www.opensource.org/licenses/mit-license.php)
