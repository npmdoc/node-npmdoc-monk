# npmdoc-monk

#### basic api documentation for  [monk (v4.0.0)](https://github.com/Automattic/monk#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-monk.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-monk) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-monk.svg)](https://travis-ci.org/npmdoc/node-npmdoc-monk)

#### [![build status](https://secure.travis-ci.org/Automattic/monk.svg?branch=master)](https://secure.travis-ci.org/Automattic/monk) [![codecov](https://codecov.io/gh/Automattic/monk/branch/master/graph/badge.svg)](https://codecov.io/gh/Automattic/monk) [![Joi

[![NPM](https://nodei.co/npm/monk.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/monk)

- [https://npmdoc.github.io/node-npmdoc-monk/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-monk/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-monk/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-monk/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-monk/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-monk/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/Automattic/monk/issues"
    },
    "dependencies": {
        "debug": "*",
        "mongodb": "^2.1.18"
    },
    "description": "[![build status](https://secure.travis-ci.org/Automattic/monk.svg?branch=master)](https://secure.travis-ci.org/Automattic/monk) [![codecov](https://codecov.io/gh/Automattic/monk/branch/master/graph/badge.svg)](https://codecov.io/gh/Automattic/monk) [![Joi",
    "devDependencies": {
        "ava": "^0.15.2",
        "codecov": "^1.0.1",
        "eslint": "^2.11.1",
        "eslint-config-standard": "^5.3.1",
        "eslint-plugin-ava": "2.5.0",
        "eslint-plugin-promise": "^1.3.2",
        "eslint-plugin-standard": "^1.3.2",
        "gitbook-cli": "2.3.0",
        "gitbook-plugin-anker-enable": "0.0.4",
        "gitbook-plugin-edit-link": "2.0.2",
        "gitbook-plugin-github": "2.0.0",
        "gitbook-plugin-prism": "1.0.0",
        "nyc": "^6.4.4"
    },
    "directories": {},
    "dist": {
        "shasum": "ac5439e3543b1b486d787d1704bd7e10a2ddd0d2",
        "tarball": "https://registry.npmjs.org/monk/-/monk-4.0.0.tgz"
    },
    "files": [
        "lib"
    ],
    "gitHead": "88caf69ad0da0d3d4691a4affa5181e290340c25",
    "homepage": "https://github.com/Automattic/monk#readme",
    "license": "MIT",
    "main": "lib/monk.js",
    "maintainers": [
        {
            "name": "mathieudutour"
        },
        {
            "name": "rauchg"
        },
        {
            "name": "tootallnate"
        }
    ],
    "name": "monk",
    "nyc": {
        "include": [
            "lib/**"
        ]
    },
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/Automattic/monk.git"
    },
    "scripts": {
        "coverage": "nyc report --reporter=text-lcov > coverage.lcov && codecov",
        "test": "make test"
    },
    "tags": [
        "mongodb",
        "mongo",
        "driver"
    ],
    "version": "4.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
