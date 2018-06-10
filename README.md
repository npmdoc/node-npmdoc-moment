# npmdoc-moment

#### basic api documentation for  [moment (2.22.2)](http://momentjs.com)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-moment.svg)](https://travis-ci.org/npmdoc/node-npmdoc-moment)

#### Parse, validate, manipulate, and display dates

[![NPM](https://nodei.co/npm/moment.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/moment)

- [https://npmdoc.github.io/node-npmdoc-moment/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-moment/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-moment/build/screenshot.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-moment/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-moment/build/screenshot.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-moment/build/screenshot.npmPackageDependencyTree.svg)



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
        "load-grunt-tasks": "~3.5.2",
        "node-qunit": "^1.0.0",
        "nyc": "^2.1.4",
        "qunit": "^2.6.0",
        "rollup": "latest",
        "spacejam": "latest",
        "typescript": "^1.8.10",
        "uglify-js": "latest"
    },
    "directories": {},
    "dist": {
        "shasum": "3c257f9839fc0e93ff53149632239eb90783ff66",
        "tarball": "https://registry.npmjs.org/moment/-/moment-2.22.2.tgz",
        "fileCount": 364,
        "unpackedSize": 2714826,
        "npm-signature": "-----BEGIN PGP SIGNATURE-----\r\nVersion: OpenPGP.js v3.0.4\r\nComment: https://openpgpjs.org\r\n\r\nwsFcBAEBCAAQBQJbEO6iCRA9TVsSAnZWagAA0UMQAKGHBnBzmDFFPcPNCaf2\nhLhTPtZ8BGfomqj1dFeSp+8dwxyiroMTJ8qRkAxKOaatayXwop7ez+kBxnMg\nPP0zoSBsX3M4ZX4FTTpH5ltvM+oBGOJT9kbMES8jeYAJBBSjD+qc9X+AmE88\nM1qGAbmSaAw6Wzu03eQ+MZ9xy9GbqeIhPkVTH2fcp1zFpoAZZYdTF+unTGv8\nGmUj7Nxwt5TlGgJS09eeivMSVOB+07YWaJc8A+bxIGAEIVfAwbbIpvItS69r\n0YnRmE4DaFg13PZJvL4gw9quCxqPpyvn7tf2C3hCyQKA+Mb2q+89wfPrBIQI\nxkKd4QM9pdNfj1f6MLGNe56E925WydQ6GatEx3RUBSgFNFwT6KmVbmhIU9Gn\nflz2Rx6zi3c9XbdvVffhw7xZtUtgWmCtBbg5nTIUBreafjGATb/RFDmJEPk+\nPTYLaf5SzHioaiPR1iFSEpgAvqU1A/a85396IhuCJ/9m3rw2fASVoYwLvfct\nD1BGqzNlctyLNThywa5h1TozFHaqtwFVSt/U5B9Fvn29zG+SYu2NOW6lcvg9\n8ip3mWjSZLkDCRawHsxVxvbTpLU2ZInnC/ym+kG/jwopd9SMcLwmLyiOXL0N\nBOHXUto0MffamsfrB/Kb0zmJHodl/y8gu7NjdzESBAQX/090cbgneXLMm9Pb\nT8lS\r\n=UATQ\r\n-----END PGP SIGNATURE-----\r\n"
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
            "name": "marwahaha"
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
    "version": "2.22.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
