# Neutrino CSSNext preset

[![Greenkeeper badge](https://badges.greenkeeper.io/barraponto/neutrino-preset-postcss-cssnext.svg)](https://greenkeeper.io/)
[![NPM version][npm-image]][npm-url] [![NPM downloads][npm-downloads]][npm-url]
[![Join Slack][slack-image]][slack-url]

`neutrino-preset-cssnext` is a Neutrino preset that adds support for
[cssnext][cssnext].

## Documentation

Install this preset to your development dependencies, then set it in
`package.json`:

```json
"neutrino": {
  "use": [
    "neutrino-preset-web",
    "neutrino-preset-cssnext"
  ]
}
```

You can configure the features through the [browsers][cssnext-browserslist]
settings (see [Browserslist query syntax][browserslist-docs]). For example, it
could be added in `package.json`:

```json
"browserslist": [
  "> 1%",
  "last 2 versions"
],
"neutrino": {
  "use": [
    "neutrino-preset-web",
    "neutrino-preset-cssnext"
  ]
}
```

## Known Issues

While the [middleware][postcss-middleware] is able to pick up PostCSS
configuration, this preset isn't. If you need to support more plugins, consider
extending this preset or the middleware directly.

[cssnext]: http://cssnext.io/
[cssnext-browserslist]: http://cssnext.io/usage/#browsers
[postcss-middleware]: https://npmjs.org/package/neutrino-middleware-postcss
[browserslist-docs]: https://github.com/ai/browserslist#queries
[npm-image]: https://img.shields.io/npm/v/neutrino-preset-cssnext.svg
[npm-downloads]: https://img.shields.io/npm/dt/neutrino-preset-cssnext.svg
[npm-url]: https://npmjs.org/package/neutrino-preset-cssnext
[slack-image]: https://neutrino-slack.herokuapp.com/badge.svg
[slack-url]: https://neutrino-slack.herokuapp.com/
