# [![stylelint-config-bigchaindb](media/repo-banner@2x.png)](https://www.bigchaindb.com)

> 💅 For consistent CSS across BigchainDB, IPDB & ascribe's repos. Extends on [stylelint-config-standard](https://github.com/stylelint/stylelint-config-standard)

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

Add this to your `.stylelintrc` file:

```json
{
    "extends": "stylelint-config-bigchaindb"
}
```

Then use `stylelint` against your css files, e.g.:

```bash
stylelint *.scss
```

Or lint in your editor with one of the many editor plugins for [stylelint](https://stylelint.io), e.g. for Atom:

```bash
apm install linter-stylelint
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
