# [![stylelint-config-bigchaindb](media/repo-banner@2x.png)](https://www.bigchaindb.com)

> 💅 For consistent CSS across BigchainDB, IPDB & ascribe's repos. Extends on [stylelint-config-standard](https://github.com/stylelint/stylelint-config-standard)

[![css bigchaindb](https://img.shields.io/badge/css-bigchaindb-39BA91.svg)](https://github.com/bigchaindb/stylelint-config-bigchaindb)
[![js bigchaindb](https://img.shields.io/badge/js-bigchaindb-39BA91.svg)](https://github.com/ascribe/javascript)
[![npm](https://img.shields.io/npm/v/stylelint-config-bigchaindb.svg)](https://www.npmjs.com/package/stylelint-config-bigchaindb)
[![Build Status](https://travis-ci.org/bigchaindb/stylelint-config-bigchaindb.svg?branch=master)](https://travis-ci.org/bigchaindb/stylelint-config-bigchaindb)
[![Greenkeeper badge](https://badges.greenkeeper.io/bigchaindb/stylelint-config-bigchaindb.svg)](https://greenkeeper.io/)

This cat clearly forgot to lint her CSS before deployment:

![cat not linting correctly](media/cat-linter-fail.gif)

Don't be like that cat.

## Installation

```bash
npm install stylelint-config-bigchaindb
```

## Usage

### Setup

Add this to your `.stylelintrc` file:

```json
{
    "extends": "stylelint-config-bigchaindb"
}
```

If you really know what you're doing™ you can change or disable individual rules globally in your project:

```json
{
    "extends": "stylelint-config-bigchaindb",
    "rules": {
        "selector-max-id": 1,
        "selector-no-qualifying-type": null
    }
}
```

Or disable blocks inline in your css:

```scss
/* stylelint-disable selector-list-comma-newline-after  */
h1, h2, h3, h4, h5, h6,
.h1, .h2, .h3, .h4, .h5, .h6 {
    color: $that-pink-which-burns-my-eyes;
}
/* stylelint-enable */
```

In general, try to never disable anything. Every time you disable even one rule one of those creatures gets killed:

![disable punishment](media/disable-punishment.gif)

### Linting

Use `stylelint` against your css files, e.g.:

```bash
stylelint *.scss
```

Or lint in your editor with one of the many editor plugins for [stylelint](https://stylelint.io), e.g. for Atom:

```bash
apm install linter-stylelint
```

## npm releases

For a new **patch release**, execute on the machine where you're logged into your npm account:

```bash
npm run release
```

Command is powered by [`release-it`](https://github.com/webpro/release-it) package, defined in the `package.json`.

That's what the command does without any user interaction:

- create release commit by updating version in `package.json`
- create tag for that release commit
- push commit & tag
- create a new release on GitHub, with change log auto-generated from commit messages
- publish to npm as a new release

If you want to create a **minor** or **major release**, use these commands:

```bash
npm run release-minor
```

```bash
npm run release-major
```

## License

```
Copyright 2017 BigchainDB GmbH

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
