<p align="center">
  <a href="https://todc.github.io/todc-bootstrap/">
    <img src="https://todc.github.io/todc-bootstrap/docs/4.3/assets/brand/todc-bootstrap-solid.svg" alt="TODC Bootstrap logo" width="72" height="72">
  </a>
</p>

<h3 align="center">TODC Bootstrap</h3>

<p align="center">
  A Google-styled theme for <a href="https://getbootstrap.com/">Bootstrap</a>.
  <br>
  <a href="https://todc.github.io/todc-bootstrap/docs/4.3/"><strong>Explore TODC Bootstrap docs »</strong></a>
  <br>
  <br>
  <a href="https://github.com/todc/todc-bootstrap/issues/new?template=bug.md">Report bug</a>
  ·
  <a href="https://github.com/todc/todc-bootstrap/issues/new?template=feature.md&labels=feature">Request feature</a>
</p>


## Table of contents

* [Overview](#overview)
* [Quick start](#quick-start)
* [Status](#status)
* [Compatibility](#compatibility)
* [Requirements](#requirements)
* [Bugs and feature requests](#bugs-and-feature-requests)
* [Documentation](#documentation)
* [Contributing](#contributing)
* [Versioning](#versioning)
* [Creators](#creators)
* [Thanks](#thanks)
* [Copyright and license](#copyright-and-license)
* [Acknowledgements](#acknowledgements)


## Overview ##

This is a Google-styled theme for Bootstrap. Because I'm a fan of the new Google UI seen in Gmail, Docs, Calendar, etc, I decided to reproduce the look of these new UI elements for my own personal use. The project's goal isn't UI parity with Google Apps -- it's feature parity with
Bootstrap, themed with Google's UI in mind.

TODC Bootstrap was created by [Tim O'Donnell](https://github.com/todc), and maintained with the support and involvement of the community.


## Quick start

Several quick start options are available:

- [Download the latest release](https://github.com/todc/todc-bootstrap/archive/v4.3.1-4.3.1.zip).
- Clone the repo: `git clone https://github.com/todc/todc-bootstrap.git`.
- Install with [npm](https://www.npmjs.com/): `npm install todc-bootstrap`
- Install with [yarn](https://yarnpkg.com/): `yarn add todc-bootstrap@4.3.1-4.3.1`
- Install with [Composer](https://getcomposer.org/): `composer require todc/todc-bootstrap:4.3.1-4.3.1`.

**NOTE** - After cloning/installing todc-bootstrap you must run `grunt checkout-bootstrap` from the todc-bootstrap directory. This will download the correct version of the [Bootstrap](https://github.com/twbs/bootstrap/) source.

Read the [Getting started page](https://todc.github.io/todc-bootstrap/docs/4.3/getting-started/introduction/) for information on the framework contents, templates and examples, and more.


## Status

**TODO - Configure BrowserStack**

[![BrowserStack Status](https://www.browserstack.com/automate/badge.svg?badge_key=SkxZcStBeExEdVJqQ2hWYnlWckpkNmNEY213SFp6WHFETWk2bGFuY3pCbz0tLXhqbHJsVlZhQnRBdEpod3NLSDMzaHc9PQ==--3d0b75245708616eb93113221beece33e680b229)](https://www.browserstack.com/automate/public-build/SkxZcStBeExEdVJqQ2hWYnlWckpkNmNEY213SFp6WHFETWk2bGFuY3pCbz0tLXhqbHJsVlZhQnRBdEpod3NLSDMzaHc9PQ==--3d0b75245708616eb93113221beece33e680b229)


### What's included

Within the download you'll find the following directories and files, logically grouping common assets and providing both compiled and minified variations. You'll see something like this:

```text
todc-bootstrap/
└── dist/
    ├── css/
    │   ├── bootstrap-grid.css
    │   ├── bootstrap-grid.css.map
    │   ├── bootstrap-grid.min.css
    │   ├── bootstrap-grid.min.css.map
    │   ├── bootstrap-reboot.css
    │   ├── bootstrap-reboot.css.map
    │   ├── bootstrap-reboot.min.css
    │   ├── bootstrap-reboot.min.css.map
    │   ├── bootstrap.css
    │   ├── bootstrap.css.map
    │   ├── bootstrap.min.css
    │   ├── bootstrap.min.css.map
    │   ├── todc-bootstrap.css
    │   ├── todc-bootstrap.css.map
    │   ├── todc-bootstrap.min.css
    │   └── todc-bootstrap.min.css.map
    └── js/
        ├── bootstrap.bundle.js
        ├── bootstrap.bundle.js.map
        ├── bootstrap.bundle.min.js
        ├── bootstrap.bundle.min.js.map
        ├── bootstrap.js
        ├── bootstrap.js.map
        ├── bootstrap.min.js
        └── bootstrap.min.js.map
```

We provide compiled CSS and JS (`bootstrap.*, todc-bootstrap.*`), as well as compiled and minified CSS and JS (`bootstrap.min.*, todc-bootstrap.min.*`). [source maps](https://developers.google.com/web/tools/chrome-devtools/javascript/source-maps) (`bootstrap.*.map, todc-bootstrap.*.map`) are available for use with certain browsers' developer tools. Bundled JS files (`bootstrap.bundle.js` and minified `bootstrap.bundle.min.js`) include [Popper](https://popper.js.org/).


## Compatibility ##

This is being tested in the latest versions of Chrome, Firefox, and IE8+.

The following projects are specifically designed for use with todc-bootstrap:

* [todc-select2](https://github.com/todc/todc-select2/) - Google-themed select menus
* [todc-datepicker](https://github.com/todc/todc-datepicker/) - Google-themed datepicker component


## Requirements ##

* [SASS](https://sass-lang.com/) - for compiling `.scss` files into CSS
* [Bootstrap](https://github.com/twbs/bootstrap/) - this will be automatically checked out, if necessary, during the build process


## Bugs and feature requests

Have a bug or a feature request? Please first read the [issue guidelines](https://github.com/todc/todc-bootstrap/blob/master/.github/CONTRIBUTING.md#using-the-issue-tracker) and search for existing and closed issues. If your problem or idea is not addressed yet, [please open a new issue](https://github.com/todc/todc-bootstrap/issues/new).


## Documentation

TODC Bootstrap's documentation, included in this repo in the root directory, is built with [Hugo](https://gohugo.io/) and publicly hosted on GitHub Pages at <https://todc.github.io/todc-bootstrap/>. The docs may also be run locally.

Documentation search is powered by [Algolia's DocSearch](https://community.algolia.com/docsearch/). Working on our search? Be sure to set `debug: true` in `site/static/docs/4.3/assets/js/src/search.js` file.

### Running documentation locally

1. Run `npm install` to install the Node.js dependencies, including Hugo (the site builder).
2. Run `npm run test` (or a specific npm script) to rebuild distributed CSS and JavaScript files, as well as our docs assets.
3. From the root `/todc-bootstrap` directory, run `npm run docs-serve` in the command line.
4. Open `http://localhost:9002/` in your browser, and voilà.

Learn more about using Hugo by reading its [documentation](https://gohugo.io/documentation/).

### Documentation for previous releases

You can find all our previous releases docs on <https://todc.github.io/todc-bootstrap/docs/versions/>.

[Previous releases](https://github.com/todc/todc-bootstrap/releases) and their documentation are also available for download.


## Contributing

Please read through our [contributing guidelines](https://github.com/todc/todc-bootstrap/blob/master/.github/CONTRIBUTING.md). Included are directions for opening issues, coding standards, and notes on development.

Editor preferences are available in the [editor config](https://github.com/todc/todc-bootstrap/blob/master/.editorconfig) for easy use in common text editors. Read more and download plugins at <https://editorconfig.org/>.


## Versioning

For transparency into our release cycle and in striving to maintain backward compatibility, Bootstrap is maintained under [the Semantic Versioning guidelines](https://semver.org/). Sometimes we screw up, but we adhere to those rules whenever possible.

See [the Releases section of our GitHub project](https://github.com/todc/todc-bootstrap/releases) for changelogs for each release version of TODC Bootstrap.

Releases will be numbered with the following format:

`<major>.<minor>.<patch>-<major>.<minor>.<patch>`

The first set of `<major>.<minor>.<patch>` is the Bootstrap version while the second set is the todc-bootstrap version.

Given a version number MAJOR.MINOR.PATCH, increment the:

* MAJOR version when you make incompatible API changes,
* MINOR version when you add functionality in a backwards-compatible manner, and
* PATCH version when you make backwards-compatible bug fixes.

Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.


## Creators

**Tim O'Donnell**

* <https://github.com/todc>


## Thanks

<a href="https://www.browserstack.com/">
  <img src="https://live.browserstack.com/images/opensource/browserstack-logo.svg" alt="BrowserStack Logo" width="192" height="42">
</a>

Thanks to [BrowserStack](https://www.browserstack.com/) for providing the infrastructure that allows us to test in real browsers!

## Copyright and license

Copyright 2011-2019 Tim O'Donnell. Code released under [the MIT license](https://github.com/todc/todc-bootstrap/blob/master/LICENSE). Docs released under [Creative Commons Attribution 3.0 Unported](https://github.com/todc/todc-bootstrap/blob/master/docs/LICENSE).

**NOTE** This project was previously and incorrectly licensed under the Public Domain. It has now been changed to be compatible with Bootstrap's current license.


## Acknowledgements ##

Inspired by [Bootstrap](https://getbootstrap.com/) and, of course, Google.
