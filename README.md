### Compendium Themer

![Latest Release Download Count](https://img.shields.io/github/downloads/p4535992/foundryvtt-compendium-themer/latest/module.zip?color=2b82fc&label=DOWNLOADS&style=for-the-badge)

[![Forge Installs](https://img.shields.io/badge/dynamic/json?label=Forge%20Installs&query=package.installs&suffix=%25&url=https%3A%2F%2Fforge-vtt.com%2Fapi%2Fbazaar%2Fpackage%2Fcompendium-themer&colorB=006400&style=for-the-badge)](https://forge-vtt.com/bazaar#package=compendium-themer)

![Foundry Core Compatible Version](https://img.shields.io/badge/dynamic/json.svg?url=https%3A%2F%2Fraw.githubusercontent.com%2Fp4535992%2Ffoundryvtt-compendium-themer%2Fmaster%2Fsrc%2Fmodule.json&label=Foundry%20Version&query=$.compatibility.verified&colorB=orange&style=for-the-badge)

![Latest Version](https://img.shields.io/badge/dynamic/json.svg?url=https%3A%2F%2Fraw.githubusercontent.com%2Fp4535992%2Ffoundryvtt-compendium-themer%2Fmaster%2Fsrc%2Fmodule.json&label=Latest%20Release&prefix=v&query=$.version&colorB=red&style=for-the-badge)

[![Foundry Hub Endorsements](https://img.shields.io/endpoint?logoColor=white&url=https%3A%2F%2Fwww.foundryvtt-hub.com%2Fwp-json%2Fhubapi%2Fv1%2Fpackage%2Fcompendium-themer%2Fshield%2Fendorsements&style=for-the-badge)](https://www.foundryvtt-hub.com/package/compendium-themer/)

![GitHub all releases](https://img.shields.io/github/downloads/p4535992/foundryvtt-compendium-themer/total?style=for-the-badge)

[![Translation status](https://weblate.foundryvtt-hub.com/widgets/compendium-themer/-/287x66-black.png)](https://weblate.foundryvtt-hub.com/engage/compendium-themer/)

### If you want to buy me a coffee [![alt-text](https://img.shields.io/badge/-Patreon-%23ff424d?style=for-the-badge)](https://www.patreon.com/p4535992)

A very little module to add some custom compendium banner images, text color and style to the compendium directory. A small module to help better search for specific module compendiums when they start to be several.

ON DEMAND you can ask me to add other modules by open a issue on the github .

### Table of supported modules

| Module ID                                             | NOTES                                           | IMAGE LICENSE DETAIL |
|-------------------------------------------------------|-------------------------------------------------|----------------------|
| [mmm](https://github.com/theripper93/Maxwell-s-Manual-of-Malicious-Maladies) | [Maxwell's Manual of Malicious Maladies - A module for all your lingering injuries needs (dnd5e)](https://drive.google.com/file/d/1z_oTJvusofehZoFKp8iDhRdZlMjWVxa_/view?usp=sharing) | [Images](/src/assets/mmm/) All images and graphics contained in this material are free use and retrieved from: [pixabay.com](https://pixabay.com/) |
| compendiums-mythos-workshop-dnd5e                     | A private compendium module | [Images](/src/assets/compendiums-mythos-workshop-dnd5e/) Image Generated with [bing create](https://www.bing.com/create) under these [term of use](https://www.bing.com/new/termsofuse?FORM=GENTOS) |
|[Broderick's Compendium: Plants and Fungi Across the Realm](https://github.com/marcstraube/foundryvtt-brodericks-compendium) | | Images recover from the module himself |

### Example

**BEFORE**

![](./wiki/before1.png)

**AFTER (without minimal css enabled)**

![](./wiki/after_without_minimal_css.png)

**AFTER (with minimal css enabled)**

![](./wiki/after_with_minimal_css.png)

## Installation

It's always easiest to install modules from the in game add-on browser.

To install this module manually:
1.  Inside the Foundry "Configuration and Setup" screen, click "Add-on Modules"
2.  Click "Install Module"
3.  In the "Manifest URL" field, paste the following url:
`https://raw.githubusercontent.com/p4535992/foundryvtt-compendium-themer/master/src/module.json`
4.  Click 'Install' and wait for installation to complete
5.  Don't forget to enable the module in game using the "Manage Module" button


## Known issue

# API

All informations about the api can be found here [API](./wiki/api/api.md)

# Build

## Install all packages

```bash
npm install
```

### dev

`dev` will let you develop you own code with hot reloading on the browser

```bash
npm run dev
```

### build

`build` will build and set up a symlink between `dist` and your `dataPath`.

```bash
npm run build
```

### build:watch

`build:watch` will build and watch for changes, rebuilding automatically.

```bash
npm run build:watch
```

### prettier-format

`prettier-format` launch the prettier plugin based on the configuration [here](./.prettierrc)

```bash
npm run-script prettier-format
```

### lint

`lint` launch the eslint process based on the configuration [here](./.eslintrc.json)

```bash
npm run-script lint
```

### lint:fix

`lint:fix` launch the eslint process with the fix argument

```bash
npm run-script lint:fix
```

### build:json

`build:json` unpack LevelDB pack on `src/packs` to the json db sources in `src/packs/_source`very useful for backup your items and manually fix some hard issue with some text editor

```bash
npm run-script build:json
```

### build:clean

`build:clean` clean packs json sources in `src/packs/_source`. NOTE: usually this command is launched after the command `build:json` and after make some modifications on the json source files with some text editor, but before the `build:db`

```bash
npm run-script build:clean
```

### build:db

`build:db` packs the json db sources in `src/packs/_source` to LevelDB pack on `src/packs` with the new jsons. NOTE: usually this command is launched after the command `build:json` and after make some modifications on the json source files with some text editor

```bash
npm run-script build:db
```

## [Changelog](./CHANGELOG.md)

## Issues

Any issues, bugs, or feature requests are always welcome to be reported directly to the [Issue Tracker](https://github.com/p4535992/foundryvtt-compendium-themer/issues ), or using the [Bug Reporter Module](https://foundryvtt.com/packages/bug-reporter/).

## License

- Images for the module [mmm](https://github.com/theripper93/Maxwell-s-Manual-of-Malicious-Maladies) with source [Maxwell's Manual of Malicious Maladies - A module for all your lingering injuries needs (dnd5e)](https://drive.google.com/file/d/1z_oTJvusofehZoFKp8iDhRdZlMjWVxa_/view?usp=sharing) in the folder [images](/src/assets/mmm/) are free use and retrieved from: [pixabay.com](https://pixabay.com/)
- Images for the module [compendiums-mythos-workshop-dnd5e]() with source a private compendium module in the folder [Images](/src/assets/compendiums-mythos-workshop-dnd5e/) are generated with [bing create](https://www.bing.com/create) under these [term of use](https://www.bing.com/new/termsofuse?FORM=GENTOS)
- Images for the module [Broderick's Compendium: Plants and Fungi Across the Realm](https://github.com/marcstraube/foundryvtt-brodericks-compendium) with source recovered from the module himself are under these [term of use](https://foundryvtt.com/article/license/)

This package is under an [MIT license](LICENSE) and the [Foundry Virtual Tabletop Limited License Agreement for module development](https://foundryvtt.com/article/license/).


