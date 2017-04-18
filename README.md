# npmdoc-moment

#### api documentation for  [moment (v2.18.1)](http://momentjs.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-moment.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-moment) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-moment.svg)](https://travis-ci.org/npmdoc/node-npmdoc-moment)

#### Parse, validate, manipulate, and display dates

[![NPM](https://nodei.co/npm/moment.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/moment)

- [https://npmdoc.github.io/node-npmdoc-moment/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-moment/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-moment/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-moment/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-moment/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-moment/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Iskren Ivov Chernev",
        "url": "https://github.com/ichernev"
    },
    "bugs": {
        "url": "https://github.com/moment/moment/issues"
    },
    "contributors": [
        {
            "name": "Tim Wood",
            "url": "http://timwoodcreates.com/"
        },
        {
            "name": "Rocky Meza",
            "url": "http://rockymeza.com"
        },
        {
            "name": "Matt Johnson",
            "url": "http://codeofmatt.com"
        },
        {
            "name": "Isaac Cambron",
            "url": "http://isaaccambron.com"
        },
        {
            "name": "Andre Polykanine",
            "url": "https://github.com/oire"
        }
    ],
    "dependencies": {},
    "description": "Parse, validate, manipulate, and display dates",
    "devDependencies": {
        "benchmark": "latest",
        "coveralls": "^2.11.2",
        "es6-promise": "latest",
        "grunt": "~0.4",
        "grunt-benchmark": "latest",
        "grunt-cli": "latest",
        "grunt-contrib-clean": "latest",
        "grunt-contrib-concat": "latest",
        "grunt-contrib-copy": "latest",
        "grunt-contrib-jshint": "latest",
        "grunt-contrib-uglify": "latest",
        "grunt-contrib-watch": "latest",
        "grunt-env": "latest",
        "grunt-exec": "latest",
        "grunt-jscs": "latest",
        "grunt-karma": "latest",
        "grunt-nuget": "latest",
        "grunt-string-replace": "latest",
        "karma": "latest",
        "karma-chrome-launcher": "latest",
        "karma-firefox-launcher": "latest",
        "karma-qunit": "latest",
        "karma-sauce-launcher": "latest",
        "load-grunt-tasks": "latest",
        "nyc": "^2.1.4",
        "qunit": "^0.7.5",
        "qunit-cli": "^0.1.4",
        "rollup": "latest",
        "spacejam": "latest",
        "typescript": "^1.8.10",
        "uglify-js": "latest"
    },
    "directories": {},
    "dist": {
        "shasum": "c36193dd3ce1c2eed2adb7c802dbbc77a81b1c0f",
        "tarball": "https://registry.npmjs.org/moment/-/moment-2.18.1.tgz"
    },
    "dojoBuild": "package.js",
    "ender": "./ender.js",
    "engines": {
        "node": "*"
    },
    "homepage": "http://momentjs.com",
    "jsnext:main": "./src/moment.js",
    "jspm": {
        "files": [
            "moment.js",
            "moment.d.ts",
            "locale"
        ],
        "map": {
            "moment": "./moment"
        },
        "buildConfig": {
            "uglify": true
        }
    },
    "keywords": [
        "moment",
        "date",
        "time",
        "parse",
        "format",
        "validate",
        "i18n",
        "l10n",
        "ender"
    ],
    "license": "MIT",
    "main": "./moment.js",
    "maintainers": [
        {
            "name": "ichernev"
        },
        {
            "name": "maggiepint"
        },
        {
            "name": "mj1856"
        },
        {
            "name": "timrwood"
        }
    ],
    "name": "moment",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/moment/moment.git"
    },
    "scripts": {
        "coverage": "nyc npm test && nyc report",
        "coveralls": "nyc npm test && nyc report --reporter=text-lcov | coveralls",
        "test": "grunt test",
        "typescript-test": "tsc --project typing-tests"
    },
    "spm": {
        "main": "moment.js",
        "output": [
            "locale/*.js"
        ]
    },
    "typings": "./moment.d.ts",
    "version": "2.18.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
