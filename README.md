# Neutralinojs v2.0.0 spec.

Neutralino v2 is ready for Linux/Windows. You can try this [pre-release](https://github.com/neutralinojs/neutralinojs/releases/tag/v2.0.0).
Please notice that the macOS version is not yet supporting v2 implementaton (still in v1.5.0). If you are interested, you can [help ❤️](https://github.com/neutralinojs/neutralinojs/issues/395) us to implement v2-spec for macOS.

## Get started 

You can create Neutralinojs v2 applications with the latest neu CLI.

Install the CLI.

```
$ npm -g install @neutralinojs/neu
```

Create a new application.

```
$ neu create myApp
$ cd myApp
```

Run your application.

```
$ neu run
```

Share it with Linux/Windows users.

```
$ neu build --release
```

## v1.x vs v2.x improvements.

- [Refactoring JavaScript API](js-api-refactoring.md) - 2/2 Done
- [settings.json -> neutralino.config.json](neutralino.config.json.md) - 2/2 Done
- [Security improvements](security.md) - 1/1 Done
- [Router improvements](router.md) - 2/2 Done
- [Project structure](project-structure.md) - 1/2 Done
- [Webview on Windows](webview.md) - 1/1 Done
