# api documentation for  [moment (v2.18.1)](http://momentjs.com)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-moment.svg)](https://travis-ci.org/npmdoc/node-npmdoc-moment)
#### Parse, validate, manipulate, and display dates

[![NPM](https://nodei.co/npm/moment.png?downloads=true)](https://www.npmjs.com/package/moment)

[![apidoc](https://npmdoc.github.io/node-npmdoc-moment/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-moment_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-moment/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-moment/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Iskren Ivov Chernev",
        "email": "iskren.chernev@gmail.com",
        "url": "https://github.com/ichernev"
    },
    "bugs": {
        "url": "https://github.com/moment/moment/issues"
    },
    "contributors": [
        {
            "name": "Tim Wood",
            "email": "washwithcare@gmail.com",
            "url": "http://timwoodcreates.com/"
        },
        {
            "name": "Rocky Meza",
            "url": "http://rockymeza.com"
        },
        {
            "name": "Matt Johnson",
            "email": "mj1856@hotmail.com",
            "url": "http://codeofmatt.com"
        },
        {
            "name": "Isaac Cambron",
            "email": "isaac@isaaccambron.com",
            "url": "http://isaaccambron.com"
        },
        {
            "name": "Andre Polykanine",
            "email": "andre@oire.org",
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
            "name": "ichernev",
            "email": "iskren.chernev@gmail.com"
        },
        {
            "name": "maggiepint",
            "email": "maggiepint@gmail.com"
        },
        {
            "name": "mj1856",
            "email": "mj1856@hotmail.com"
        },
        {
            "name": "timrwood",
            "email": "washwithcare@gmail.com"
        }
    ],
    "name": "moment",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module moment](#apidoc.module.moment)
1.  boolean <span class="apidocSignatureSpan">moment.</span>suppressDeprecationWarnings
1.  [function <span class="apidocSignatureSpan">moment.</span>ISO_8601 ()](#apidoc.element.moment.ISO_8601)
1.  [function <span class="apidocSignatureSpan">moment.</span>RFC_2822 ()](#apidoc.element.moment.RFC_2822)
1.  [function <span class="apidocSignatureSpan">moment.</span>calendarFormat (myMoment, now)](#apidoc.element.moment.calendarFormat)
1.  [function <span class="apidocSignatureSpan">moment.</span>createFromInputFallback ()](#apidoc.element.moment.createFromInputFallback)
1.  [function <span class="apidocSignatureSpan">moment.</span>defineLocale (name, config)](#apidoc.element.moment.defineLocale)
1.  [function <span class="apidocSignatureSpan">moment.</span>duration (input, key)](#apidoc.element.moment.duration)
1.  [function <span class="apidocSignatureSpan">moment.</span>invalid (flags)](#apidoc.element.moment.invalid)
1.  [function <span class="apidocSignatureSpan">moment.</span>isDate (input)](#apidoc.element.moment.isDate)
1.  [function <span class="apidocSignatureSpan">moment.</span>isDuration (obj)](#apidoc.element.moment.isDuration)
1.  [function <span class="apidocSignatureSpan">moment.</span>isMoment (obj)](#apidoc.element.moment.isMoment)
1.  [function <span class="apidocSignatureSpan">moment.</span>lang ()](#apidoc.element.moment.lang)
1.  [function <span class="apidocSignatureSpan">moment.</span>langData ()](#apidoc.element.moment.langData)
1.  [function <span class="apidocSignatureSpan">moment.</span>locale (key, values)](#apidoc.element.moment.locale)
1.  [function <span class="apidocSignatureSpan">moment.</span>localeData (key)](#apidoc.element.moment.localeData)
1.  [function <span class="apidocSignatureSpan">moment.</span>locales ()](#apidoc.element.moment.locales)
1.  [function <span class="apidocSignatureSpan">moment.</span>max ()](#apidoc.element.moment.max)
1.  [function <span class="apidocSignatureSpan">moment.</span>min ()](#apidoc.element.moment.min)
1.  [function <span class="apidocSignatureSpan">moment.</span>months (format, index)](#apidoc.element.moment.months)
1.  [function <span class="apidocSignatureSpan">moment.</span>monthsShort (format, index)](#apidoc.element.moment.monthsShort)
1.  [function <span class="apidocSignatureSpan">moment.</span>normalizeUnits (units)](#apidoc.element.moment.normalizeUnits)
1.  [function <span class="apidocSignatureSpan">moment.</span>now ()](#apidoc.element.moment.now)
1.  [function <span class="apidocSignatureSpan">moment.</span>parseTwoDigitYear (input)](#apidoc.element.moment.parseTwoDigitYear)
1.  [function <span class="apidocSignatureSpan">moment.</span>parseZone ()](#apidoc.element.moment.parseZone)
1.  [function <span class="apidocSignatureSpan">moment.</span>relativeTimeRounding (roundingFunction)](#apidoc.element.moment.relativeTimeRounding)
1.  [function <span class="apidocSignatureSpan">moment.</span>relativeTimeThreshold (threshold, limit)](#apidoc.element.moment.relativeTimeThreshold)
1.  [function <span class="apidocSignatureSpan">moment.</span>unix (input)](#apidoc.element.moment.unix)
1.  [function <span class="apidocSignatureSpan">moment.</span>updateLocale (name, config)](#apidoc.element.moment.updateLocale)
1.  [function <span class="apidocSignatureSpan">moment.</span>updateOffset ()](#apidoc.element.moment.updateOffset)
1.  [function <span class="apidocSignatureSpan">moment.</span>utc (input, format, locale, strict)](#apidoc.element.moment.utc)
1.  [function <span class="apidocSignatureSpan">moment.</span>weekdays (localeSorted, format, index)](#apidoc.element.moment.weekdays)
1.  [function <span class="apidocSignatureSpan">moment.</span>weekdaysMin (localeSorted, format, index)](#apidoc.element.moment.weekdaysMin)
1.  [function <span class="apidocSignatureSpan">moment.</span>weekdaysShort (localeSorted, format, index)](#apidoc.element.moment.weekdaysShort)
1.  object <span class="apidocSignatureSpan">moment.</span>deprecationHandler
1.  object <span class="apidocSignatureSpan">moment.</span>duration.fn
1.  object <span class="apidocSignatureSpan">moment.</span>fn
1.  object <span class="apidocSignatureSpan">moment.</span>momentProperties
1.  string <span class="apidocSignatureSpan">moment.</span>defaultFormat
1.  string <span class="apidocSignatureSpan">moment.</span>defaultFormatUtc
1.  string <span class="apidocSignatureSpan">moment.</span>version

#### [module moment.duration](#apidoc.module.moment.duration)
1.  [function <span class="apidocSignatureSpan">moment.</span>duration (input, key)](#apidoc.element.moment.duration.duration)
1.  [function <span class="apidocSignatureSpan">moment.duration.</span>invalid ()](#apidoc.element.moment.duration.invalid)
1.  object <span class="apidocSignatureSpan">moment.duration.</span>fn

#### [module moment.duration.fn](#apidoc.module.moment.duration.fn)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>_bubble ()](#apidoc.element.moment.duration.fn._bubble)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>abs ()](#apidoc.element.moment.duration.fn.abs)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>add (input, value)](#apidoc.element.moment.duration.fn.add)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>as (units)](#apidoc.element.moment.duration.fn.as)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>asDays ()](#apidoc.element.moment.duration.fn.asDays)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>asHours ()](#apidoc.element.moment.duration.fn.asHours)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>asMilliseconds ()](#apidoc.element.moment.duration.fn.asMilliseconds)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>asMinutes ()](#apidoc.element.moment.duration.fn.asMinutes)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>asMonths ()](#apidoc.element.moment.duration.fn.asMonths)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>asSeconds ()](#apidoc.element.moment.duration.fn.asSeconds)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>asWeeks ()](#apidoc.element.moment.duration.fn.asWeeks)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>asYears ()](#apidoc.element.moment.duration.fn.asYears)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>days ()](#apidoc.element.moment.duration.fn.days)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>get (units)](#apidoc.element.moment.duration.fn.get)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>hours ()](#apidoc.element.moment.duration.fn.hours)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>humanize (withSuffix)](#apidoc.element.moment.duration.fn.humanize)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>isValid ()](#apidoc.element.moment.duration.fn.isValid)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>lang ()](#apidoc.element.moment.duration.fn.lang)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>locale (key)](#apidoc.element.moment.duration.fn.locale)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>localeData ()](#apidoc.element.moment.duration.fn.localeData)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>milliseconds ()](#apidoc.element.moment.duration.fn.milliseconds)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>minutes ()](#apidoc.element.moment.duration.fn.minutes)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>months ()](#apidoc.element.moment.duration.fn.months)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>seconds ()](#apidoc.element.moment.duration.fn.seconds)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>subtract (input, value)](#apidoc.element.moment.duration.fn.subtract)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>toISOString ()](#apidoc.element.moment.duration.fn.toISOString)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>toIsoString ()](#apidoc.element.moment.duration.fn.toIsoString)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>toJSON ()](#apidoc.element.moment.duration.fn.toJSON)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>toString ()](#apidoc.element.moment.duration.fn.toString)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>valueOf ()](#apidoc.element.moment.duration.fn.valueOf)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>weeks ()](#apidoc.element.moment.duration.fn.weeks)
1.  [function <span class="apidocSignatureSpan">moment.duration.fn.</span>years ()](#apidoc.element.moment.duration.fn.years)



# <a name="apidoc.module.moment"></a>[module moment](#apidoc.module.moment)

#### <a name="apidoc.element.moment.ISO_8601"></a>[function <span class="apidocSignatureSpan">moment.</span>ISO_8601 ()](#apidoc.element.moment.ISO_8601)
- description and source-code
```javascript
ISO_8601 = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.RFC_2822"></a>[function <span class="apidocSignatureSpan">moment.</span>RFC_2822 ()](#apidoc.element.moment.RFC_2822)
- description and source-code
```javascript
RFC_2822 = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.calendarFormat"></a>[function <span class="apidocSignatureSpan">moment.</span>calendarFormat (myMoment, now)](#apidoc.element.moment.calendarFormat)
- description and source-code
```javascript
function getCalendarFormat(myMoment, now) {
    var diff = myMoment.diff(now, 'days', true);
    return diff < -6 ? 'sameElse' :
            diff < -1 ? 'lastWeek' :
            diff < 0 ? 'lastDay' :
            diff < 1 ? 'sameDay' :
            diff < 2 ? 'nextDay' :
            diff < 7 ? 'nextWeek' : 'sameElse';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.createFromInputFallback"></a>[function <span class="apidocSignatureSpan">moment.</span>createFromInputFallback ()](#apidoc.element.moment.createFromInputFallback)
- description and source-code
```javascript
createFromInputFallback = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.defineLocale"></a>[function <span class="apidocSignatureSpan">moment.</span>defineLocale (name, config)](#apidoc.element.moment.defineLocale)
- description and source-code
```javascript
function defineLocale(name, config) {
    if (config !== null) {
        var parentConfig = baseConfig;
        config.abbr = name;
        if (locales[name] != null) {
            deprecateSimple('defineLocaleOverride',
                    'use moment.updateLocale(localeName, config) to change ' +
                    'an existing locale. moment.defineLocale(localeName, ' +
                    'config) should only be used for creating a new locale ' +
                    'See http://momentjs.com/guides/#/warnings/define-locale/ for more info.');
            parentConfig = locales[name]._config;
        } else if (config.parentLocale != null) {
            if (locales[config.parentLocale] != null) {
                parentConfig = locales[config.parentLocale]._config;
            } else {
                if (!localeFamilies[config.parentLocale]) {
                    localeFamilies[config.parentLocale] = [];
                }
                localeFamilies[config.parentLocale].push({
                    name: name,
                    config: config
                });
                return null;
            }
        }
        locales[name] = new Locale(mergeConfigs(parentConfig, config));

        if (localeFamilies[name]) {
            localeFamilies[name].forEach(function (x) {
                defineLocale(x.name, x.config);
            });
        }

        // backwards compat for now: also set the locale
        // make sure we set the locale AFTER all child locales have been
        // created, so we won't end up with the child locale set.
        getSetGlobalLocale(name);


        return locales[name];
    } else {
        // useful for testing
        delete locales[name];
        return null;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration"></a>[function <span class="apidocSignatureSpan">moment.</span>duration (input, key)](#apidoc.element.moment.duration)
- description and source-code
```javascript
function createDuration(input, key) {
    var duration = input,
        // matching against regexp is expensive, do it on demand
        match = null,
        sign,
        ret,
        diffRes;

    if (isDuration(input)) {
        duration = {
            ms : input._milliseconds,
            d  : input._days,
            M  : input._months
        };
    } else if (isNumber(input)) {
        duration = {};
        if (key) {
            duration[key] = input;
        } else {
            duration.milliseconds = input;
        }
    } else if (!!(match = aspNetRegex.exec(input))) {
        sign = (match[1] === '-') ? -1 : 1;
        duration = {
            y  : 0,
            d  : toInt(match[DATE])                         * sign,
            h  : toInt(match[HOUR])                         * sign,
            m  : toInt(match[MINUTE])                       * sign,
            s  : toInt(match[SECOND])                       * sign,
            ms : toInt(absRound(match[MILLISECOND] * 1000)) * sign // the millisecond decimal point is included in the match
        };
    } else if (!!(match = isoRegex.exec(input))) {
        sign = (match[1] === '-') ? -1 : 1;
        duration = {
            y : parseIso(match[2], sign),
            M : parseIso(match[3], sign),
            w : parseIso(match[4], sign),
            d : parseIso(match[5], sign),
            h : parseIso(match[6], sign),
            m : parseIso(match[7], sign),
            s : parseIso(match[8], sign)
        };
    } else if (duration == null) {// checks for null or undefined
        duration = {};
    } else if (typeof duration === 'object' && ('from' in duration || 'to' in duration)) {
        diffRes = momentsDifference(createLocal(duration.from), createLocal(duration.to));

        duration = {};
        duration.ms = diffRes.milliseconds;
        duration.M = diffRes.months;
    }

    ret = new Duration(duration);

    if (isDuration(input) && hasOwnProp(input, '_locale')) {
        ret._locale = input._locale;
    }

    return ret;
}
```
- example usage
```shell
...

 * Changed language ordinal method to return the number + ordinal instead of just the ordinal.

 * Changed two digit year parsing cutoff to match strptime.

 * Removed 'moment#sod' and 'moment#eod' in favor of 'moment#startOf' and 'moment#endOf'.

 * Removed 'moment.humanizeDuration()' in favor of 'moment.duration().humanize()'.

 * Removed the lang data objects from the top level namespace.

 * Duplicate 'Date' passed to 'moment()' instead of referencing it.

## [Changelog](https://github.com/moment/moment/blob/develop/CHANGELOG.md)
...
```

#### <a name="apidoc.element.moment.invalid"></a>[function <span class="apidocSignatureSpan">moment.</span>invalid (flags)](#apidoc.element.moment.invalid)
- description and source-code
```javascript
function createInvalid(flags) {
    var m = createUTC(NaN);
    if (flags != null) {
        extend(getParsingFlags(m), flags);
    }
    else {
        getParsingFlags(m).userInvalidated = true;
    }

    return m;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.isDate"></a>[function <span class="apidocSignatureSpan">moment.</span>isDate (input)](#apidoc.element.moment.isDate)
- description and source-code
```javascript
function isDate(input) {
    return input instanceof Date || Object.prototype.toString.call(input) === '[object Date]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.isDuration"></a>[function <span class="apidocSignatureSpan">moment.</span>isDuration (obj)](#apidoc.element.moment.isDuration)
- description and source-code
```javascript
function isDuration(obj) {
    return obj instanceof Duration;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.isMoment"></a>[function <span class="apidocSignatureSpan">moment.</span>isMoment (obj)](#apidoc.element.moment.isMoment)
- description and source-code
```javascript
function isMoment(obj) {
    return obj instanceof Moment || (obj != null && obj._isAMomentObject != null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.lang"></a>[function <span class="apidocSignatureSpan">moment.</span>lang ()](#apidoc.element.moment.lang)
- description and source-code
```javascript
lang = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.langData"></a>[function <span class="apidocSignatureSpan">moment.</span>langData ()](#apidoc.element.moment.langData)
- description and source-code
```javascript
langData = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.locale"></a>[function <span class="apidocSignatureSpan">moment.</span>locale (key, values)](#apidoc.element.moment.locale)
- description and source-code
```javascript
function getSetGlobalLocale(key, values) {
    var data;
    if (key) {
        if (isUndefined(values)) {
            data = getLocale(key);
        }
        else {
            data = defineLocale(key, values);
        }

        if (data) {
            // moment.duration._locale = moment._locale = data;
            globalLocale = data;
        }
    }

    return globalLocale._abbr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.localeData"></a>[function <span class="apidocSignatureSpan">moment.</span>localeData (key)](#apidoc.element.moment.localeData)
- description and source-code
```javascript
function getLocale(key) {
    var locale;

    if (key && key._locale && key._locale._abbr) {
        key = key._locale._abbr;
    }

    if (!key) {
        return globalLocale;
    }

    if (!isArray(key)) {
        //short-circuit everything else
        locale = loadLocale(key);
        if (locale) {
            return locale;
        }
        key = [key];
    }

    return chooseLocale(key);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.locales"></a>[function <span class="apidocSignatureSpan">moment.</span>locales ()](#apidoc.element.moment.locales)
- description and source-code
```javascript
function listLocales() {
    return keys$1(locales);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.max"></a>[function <span class="apidocSignatureSpan">moment.</span>max ()](#apidoc.element.moment.max)
- description and source-code
```javascript
function max() {
    var args = [].slice.call(arguments, 0);

    return pickBy('isAfter', args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.min"></a>[function <span class="apidocSignatureSpan">moment.</span>min ()](#apidoc.element.moment.min)
- description and source-code
```javascript
function min() {
    var args = [].slice.call(arguments, 0);

    return pickBy('isBefore', args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.months"></a>[function <span class="apidocSignatureSpan">moment.</span>months (format, index)](#apidoc.element.moment.months)
- description and source-code
```javascript
function listMonths(format, index) {
    return listMonthsImpl(format, index, 'months');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.monthsShort"></a>[function <span class="apidocSignatureSpan">moment.</span>monthsShort (format, index)](#apidoc.element.moment.monthsShort)
- description and source-code
```javascript
function listMonthsShort(format, index) {
    return listMonthsImpl(format, index, 'monthsShort');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.normalizeUnits"></a>[function <span class="apidocSignatureSpan">moment.</span>normalizeUnits (units)](#apidoc.element.moment.normalizeUnits)
- description and source-code
```javascript
function normalizeUnits(units) {
    return typeof units === 'string' ? aliases[units] || aliases[units.toLowerCase()] : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.now"></a>[function <span class="apidocSignatureSpan">moment.</span>now ()](#apidoc.element.moment.now)
- description and source-code
```javascript
now = function () {
    return Date.now ? Date.now() : +(new Date());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.parseTwoDigitYear"></a>[function <span class="apidocSignatureSpan">moment.</span>parseTwoDigitYear (input)](#apidoc.element.moment.parseTwoDigitYear)
- description and source-code
```javascript
parseTwoDigitYear = function (input) {
    return toInt(input) + (toInt(input) > 68 ? 1900 : 2000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.parseZone"></a>[function <span class="apidocSignatureSpan">moment.</span>parseZone ()](#apidoc.element.moment.parseZone)
- description and source-code
```javascript
function createInZone() {
    return createLocal.apply(null, arguments).parseZone();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.relativeTimeRounding"></a>[function <span class="apidocSignatureSpan">moment.</span>relativeTimeRounding (roundingFunction)](#apidoc.element.moment.relativeTimeRounding)
- description and source-code
```javascript
function getSetRelativeTimeRounding(roundingFunction) {
    if (roundingFunction === undefined) {
        return round;
    }
    if (typeof(roundingFunction) === 'function') {
        round = roundingFunction;
        return true;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.relativeTimeThreshold"></a>[function <span class="apidocSignatureSpan">moment.</span>relativeTimeThreshold (threshold, limit)](#apidoc.element.moment.relativeTimeThreshold)
- description and source-code
```javascript
function getSetRelativeTimeThreshold(threshold, limit) {
    if (thresholds[threshold] === undefined) {
        return false;
    }
    if (limit === undefined) {
        return thresholds[threshold];
    }
    thresholds[threshold] = limit;
    if (threshold === 's') {
        thresholds.ss = limit - 1;
    }
    return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.unix"></a>[function <span class="apidocSignatureSpan">moment.</span>unix (input)](#apidoc.element.moment.unix)
- description and source-code
```javascript
function createUnix(input) {
    return createLocal(input * 1000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.updateLocale"></a>[function <span class="apidocSignatureSpan">moment.</span>updateLocale (name, config)](#apidoc.element.moment.updateLocale)
- description and source-code
```javascript
function updateLocale(name, config) {
    if (config != null) {
        var locale, parentConfig = baseConfig;
        // MERGE
        if (locales[name] != null) {
            parentConfig = locales[name]._config;
        }
        config = mergeConfigs(parentConfig, config);
        locale = new Locale(config);
        locale.parentLocale = locales[name];
        locales[name] = locale;

        // backwards compat for now: also set the locale
        getSetGlobalLocale(name);
    } else {
        // pass null for config to unupdate, useful for tests
        if (locales[name] != null) {
            if (locales[name].parentLocale != null) {
                locales[name] = locales[name].parentLocale;
            } else if (locales[name] != null) {
                delete locales[name];
            }
        }
    }
    return locales[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.updateOffset"></a>[function <span class="apidocSignatureSpan">moment.</span>updateOffset ()](#apidoc.element.moment.updateOffset)
- description and source-code
```javascript
updateOffset = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.utc"></a>[function <span class="apidocSignatureSpan">moment.</span>utc (input, format, locale, strict)](#apidoc.element.moment.utc)
- description and source-code
```javascript
function createUTC(input, format, locale, strict) {
    return createLocalOrUTC(input, format, locale, strict, true).utc();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.weekdays"></a>[function <span class="apidocSignatureSpan">moment.</span>weekdays (localeSorted, format, index)](#apidoc.element.moment.weekdays)
- description and source-code
```javascript
function listWeekdays(localeSorted, format, index) {
    return listWeekdaysImpl(localeSorted, format, index, 'weekdays');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.weekdaysMin"></a>[function <span class="apidocSignatureSpan">moment.</span>weekdaysMin (localeSorted, format, index)](#apidoc.element.moment.weekdaysMin)
- description and source-code
```javascript
function listWeekdaysMin(localeSorted, format, index) {
    return listWeekdaysImpl(localeSorted, format, index, 'weekdaysMin');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.weekdaysShort"></a>[function <span class="apidocSignatureSpan">moment.</span>weekdaysShort (localeSorted, format, index)](#apidoc.element.moment.weekdaysShort)
- description and source-code
```javascript
function listWeekdaysShort(localeSorted, format, index) {
    return listWeekdaysImpl(localeSorted, format, index, 'weekdaysShort');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.moment.duration"></a>[module moment.duration](#apidoc.module.moment.duration)

#### <a name="apidoc.element.moment.duration.duration"></a>[function <span class="apidocSignatureSpan">moment.</span>duration (input, key)](#apidoc.element.moment.duration.duration)
- description and source-code
```javascript
function createDuration(input, key) {
    var duration = input,
        // matching against regexp is expensive, do it on demand
        match = null,
        sign,
        ret,
        diffRes;

    if (isDuration(input)) {
        duration = {
            ms : input._milliseconds,
            d  : input._days,
            M  : input._months
        };
    } else if (isNumber(input)) {
        duration = {};
        if (key) {
            duration[key] = input;
        } else {
            duration.milliseconds = input;
        }
    } else if (!!(match = aspNetRegex.exec(input))) {
        sign = (match[1] === '-') ? -1 : 1;
        duration = {
            y  : 0,
            d  : toInt(match[DATE])                         * sign,
            h  : toInt(match[HOUR])                         * sign,
            m  : toInt(match[MINUTE])                       * sign,
            s  : toInt(match[SECOND])                       * sign,
            ms : toInt(absRound(match[MILLISECOND] * 1000)) * sign // the millisecond decimal point is included in the match
        };
    } else if (!!(match = isoRegex.exec(input))) {
        sign = (match[1] === '-') ? -1 : 1;
        duration = {
            y : parseIso(match[2], sign),
            M : parseIso(match[3], sign),
            w : parseIso(match[4], sign),
            d : parseIso(match[5], sign),
            h : parseIso(match[6], sign),
            m : parseIso(match[7], sign),
            s : parseIso(match[8], sign)
        };
    } else if (duration == null) {// checks for null or undefined
        duration = {};
    } else if (typeof duration === 'object' && ('from' in duration || 'to' in duration)) {
        diffRes = momentsDifference(createLocal(duration.from), createLocal(duration.to));

        duration = {};
        duration.ms = diffRes.milliseconds;
        duration.M = diffRes.months;
    }

    ret = new Duration(duration);

    if (isDuration(input) && hasOwnProp(input, '_locale')) {
        ret._locale = input._locale;
    }

    return ret;
}
```
- example usage
```shell
...

 * Changed language ordinal method to return the number + ordinal instead of just the ordinal.

 * Changed two digit year parsing cutoff to match strptime.

 * Removed 'moment#sod' and 'moment#eod' in favor of 'moment#startOf' and 'moment#endOf'.

 * Removed 'moment.humanizeDuration()' in favor of 'moment.duration().humanize()'.

 * Removed the lang data objects from the top level namespace.

 * Duplicate 'Date' passed to 'moment()' instead of referencing it.

## [Changelog](https://github.com/moment/moment/blob/develop/CHANGELOG.md)
...
```

#### <a name="apidoc.element.moment.duration.invalid"></a>[function <span class="apidocSignatureSpan">moment.duration.</span>invalid ()](#apidoc.element.moment.duration.invalid)
- description and source-code
```javascript
function createInvalid$1() {
    return createDuration(NaN);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.moment.duration.fn"></a>[module moment.duration.fn](#apidoc.module.moment.duration.fn)

#### <a name="apidoc.element.moment.duration.fn._bubble"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>_bubble ()](#apidoc.element.moment.duration.fn._bubble)
- description and source-code
```javascript
function bubble() {
    var milliseconds = this._milliseconds;
    var days         = this._days;
    var months       = this._months;
    var data         = this._data;
    var seconds, minutes, hours, years, monthsFromDays;

    // if we have a mix of positive and negative values, bubble down first
    // check: https://github.com/moment/moment/issues/2166
    if (!((milliseconds >= 0 && days >= 0 && months >= 0) ||
            (milliseconds <= 0 && days <= 0 && months <= 0))) {
        milliseconds += absCeil(monthsToDays(months) + days) * 864e5;
        days = 0;
        months = 0;
    }

    // The following code bubbles up values, see the tests for
    // examples of what that means.
    data.milliseconds = milliseconds % 1000;

    seconds           = absFloor(milliseconds / 1000);
    data.seconds      = seconds % 60;

    minutes           = absFloor(seconds / 60);
    data.minutes      = minutes % 60;

    hours             = absFloor(minutes / 60);
    data.hours        = hours % 24;

    days += absFloor(hours / 24);

    // convert days to months
    monthsFromDays = absFloor(daysToMonths(days));
    months += monthsFromDays;
    days -= absCeil(monthsToDays(monthsFromDays));

    // 12 months -> 1 year
    years = absFloor(months / 12);
    months %= 12;

    data.days   = days;
    data.months = months;
    data.years  = years;

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.abs"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>abs ()](#apidoc.element.moment.duration.fn.abs)
- description and source-code
```javascript
function abs() {
    var data           = this._data;

    this._milliseconds = mathAbs(this._milliseconds);
    this._days         = mathAbs(this._days);
    this._months       = mathAbs(this._months);

    data.milliseconds  = mathAbs(data.milliseconds);
    data.seconds       = mathAbs(data.seconds);
    data.minutes       = mathAbs(data.minutes);
    data.hours         = mathAbs(data.hours);
    data.months        = mathAbs(data.months);
    data.years         = mathAbs(data.years);

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.add"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>add (input, value)](#apidoc.element.moment.duration.fn.add)
- description and source-code
```javascript
function add$1(input, value) {
    return addSubtract$1(this, input, value, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.as"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>as (units)](#apidoc.element.moment.duration.fn.as)
- description and source-code
```javascript
function as(units) {
    if (!this.isValid()) {
        return NaN;
    }
    var days;
    var months;
    var milliseconds = this._milliseconds;

    units = normalizeUnits(units);

    if (units === 'month' || units === 'year') {
        days   = this._days   + milliseconds / 864e5;
        months = this._months + daysToMonths(days);
        return units === 'month' ? months : months / 12;
    } else {
        // handle milliseconds separately because of floating point math errors (issue #1867)
        days = this._days + Math.round(monthsToDays(this._months));
        switch (units) {
            case 'week'   : return days / 7     + milliseconds / 6048e5;
            case 'day'    : return days         + milliseconds / 864e5;
            case 'hour'   : return days * 24    + milliseconds / 36e5;
            case 'minute' : return days * 1440  + milliseconds / 6e4;
            case 'second' : return days * 86400 + milliseconds / 1000;
            // Math.floor prevents floating point math errors here
            case 'millisecond': return Math.floor(days * 864e5) + milliseconds;
            default: throw new Error('Unknown unit ' + units);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.asDays"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>asDays ()](#apidoc.element.moment.duration.fn.asDays)
- description and source-code
```javascript
asDays = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.asHours"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>asHours ()](#apidoc.element.moment.duration.fn.asHours)
- description and source-code
```javascript
asHours = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.asMilliseconds"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>asMilliseconds ()](#apidoc.element.moment.duration.fn.asMilliseconds)
- description and source-code
```javascript
asMilliseconds = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.asMinutes"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>asMinutes ()](#apidoc.element.moment.duration.fn.asMinutes)
- description and source-code
```javascript
asMinutes = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.asMonths"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>asMonths ()](#apidoc.element.moment.duration.fn.asMonths)
- description and source-code
```javascript
asMonths = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.asSeconds"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>asSeconds ()](#apidoc.element.moment.duration.fn.asSeconds)
- description and source-code
```javascript
asSeconds = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.asWeeks"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>asWeeks ()](#apidoc.element.moment.duration.fn.asWeeks)
- description and source-code
```javascript
asWeeks = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.asYears"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>asYears ()](#apidoc.element.moment.duration.fn.asYears)
- description and source-code
```javascript
asYears = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.days"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>days ()](#apidoc.element.moment.duration.fn.days)
- description and source-code
```javascript
days = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.get"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>get (units)](#apidoc.element.moment.duration.fn.get)
- description and source-code
```javascript
function get$2(units) {
    units = normalizeUnits(units);
    return this.isValid() ? this[units + 's']() : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.hours"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>hours ()](#apidoc.element.moment.duration.fn.hours)
- description and source-code
```javascript
hours = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.humanize"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>humanize (withSuffix)](#apidoc.element.moment.duration.fn.humanize)
- description and source-code
```javascript
function humanize(withSuffix) {
    if (!this.isValid()) {
        return this.localeData().invalidDate();
    }

    var locale = this.localeData();
    var output = relativeTime$1(this, !withSuffix, locale);

    if (withSuffix) {
        output = locale.pastFuture(+this, output);
    }

    return locale.postformat(output);
}
```
- example usage
```shell
...

 * Changed language ordinal method to return the number + ordinal instead of just the ordinal.

 * Changed two digit year parsing cutoff to match strptime.

 * Removed 'moment#sod' and 'moment#eod' in favor of 'moment#startOf' and 'moment#endOf'.

 * Removed 'moment.humanizeDuration()' in favor of 'moment.duration().humanize()'.

 * Removed the lang data objects from the top level namespace.

 * Duplicate 'Date' passed to 'moment()' instead of referencing it.

## [Changelog](https://github.com/moment/moment/blob/develop/CHANGELOG.md)
...
```

#### <a name="apidoc.element.moment.duration.fn.isValid"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>isValid ()](#apidoc.element.moment.duration.fn.isValid)
- description and source-code
```javascript
function isValid$1() {
    return this._isValid;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.lang"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>lang ()](#apidoc.element.moment.duration.fn.lang)
- description and source-code
```javascript
lang = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.locale"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>locale (key)](#apidoc.element.moment.duration.fn.locale)
- description and source-code
```javascript
function locale(key) {
    var newLocaleData;

    if (key === undefined) {
        return this._locale._abbr;
    } else {
        newLocaleData = getLocale(key);
        if (newLocaleData != null) {
            this._locale = newLocaleData;
        }
        return this;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.localeData"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>localeData ()](#apidoc.element.moment.duration.fn.localeData)
- description and source-code
```javascript
function localeData() {
    return this._locale;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.milliseconds"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>milliseconds ()](#apidoc.element.moment.duration.fn.milliseconds)
- description and source-code
```javascript
milliseconds = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.minutes"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>minutes ()](#apidoc.element.moment.duration.fn.minutes)
- description and source-code
```javascript
minutes = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.months"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>months ()](#apidoc.element.moment.duration.fn.months)
- description and source-code
```javascript
months = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.seconds"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>seconds ()](#apidoc.element.moment.duration.fn.seconds)
- description and source-code
```javascript
seconds = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.subtract"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>subtract (input, value)](#apidoc.element.moment.duration.fn.subtract)
- description and source-code
```javascript
function subtract$1(input, value) {
    return addSubtract$1(this, input, value, -1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.toISOString"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>toISOString ()](#apidoc.element.moment.duration.fn.toISOString)
- description and source-code
```javascript
function toISOString$1() {
    // for ISO strings we do not use the normal bubbling rules:
    //  * milliseconds bubble up until they become hours
    //  * days do not bubble at all
    //  * months bubble up until they become years
    // This is because there is no context-free conversion between hours and days
    // (think of clock changes)
    // and also not between days and months (28-31 days per month)
    if (!this.isValid()) {
        return this.localeData().invalidDate();
    }

    var seconds = abs$1(this._milliseconds) / 1000;
    var days         = abs$1(this._days);
    var months       = abs$1(this._months);
    var minutes, hours, years;

    // 3600 seconds -> 60 minutes -> 1 hour
    minutes           = absFloor(seconds / 60);
    hours             = absFloor(minutes / 60);
    seconds %= 60;
    minutes %= 60;

    // 12 months -> 1 year
    years  = absFloor(months / 12);
    months %= 12;


    // inspired by https://github.com/dordille/moment-isoduration/blob/master/moment.isoduration.js
    var Y = years;
    var M = months;
    var D = days;
    var h = hours;
    var m = minutes;
    var s = seconds;
    var total = this.asSeconds();

    if (!total) {
        // this is the same as C#'s (Noda) and python (isodate)...
        // but not other JS (goog.date)
        return 'P0D';
    }

    return (total < 0 ? '-' : '') +
        'P' +
        (Y ? Y + 'Y' : '') +
        (M ? M + 'M' : '') +
        (D ? D + 'D' : '') +
        ((h || m || s) ? 'T' : '') +
        (h ? h + 'H' : '') +
        (m ? m + 'M' : '') +
        (s ? s + 'S' : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.toIsoString"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>toIsoString ()](#apidoc.element.moment.duration.fn.toIsoString)
- description and source-code
```javascript
toIsoString = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.toJSON"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>toJSON ()](#apidoc.element.moment.duration.fn.toJSON)
- description and source-code
```javascript
function toISOString$1() {
    // for ISO strings we do not use the normal bubbling rules:
    //  * milliseconds bubble up until they become hours
    //  * days do not bubble at all
    //  * months bubble up until they become years
    // This is because there is no context-free conversion between hours and days
    // (think of clock changes)
    // and also not between days and months (28-31 days per month)
    if (!this.isValid()) {
        return this.localeData().invalidDate();
    }

    var seconds = abs$1(this._milliseconds) / 1000;
    var days         = abs$1(this._days);
    var months       = abs$1(this._months);
    var minutes, hours, years;

    // 3600 seconds -> 60 minutes -> 1 hour
    minutes           = absFloor(seconds / 60);
    hours             = absFloor(minutes / 60);
    seconds %= 60;
    minutes %= 60;

    // 12 months -> 1 year
    years  = absFloor(months / 12);
    months %= 12;


    // inspired by https://github.com/dordille/moment-isoduration/blob/master/moment.isoduration.js
    var Y = years;
    var M = months;
    var D = days;
    var h = hours;
    var m = minutes;
    var s = seconds;
    var total = this.asSeconds();

    if (!total) {
        // this is the same as C#'s (Noda) and python (isodate)...
        // but not other JS (goog.date)
        return 'P0D';
    }

    return (total < 0 ? '-' : '') +
        'P' +
        (Y ? Y + 'Y' : '') +
        (M ? M + 'M' : '') +
        (D ? D + 'D' : '') +
        ((h || m || s) ? 'T' : '') +
        (h ? h + 'H' : '') +
        (m ? m + 'M' : '') +
        (s ? s + 'S' : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.toString"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>toString ()](#apidoc.element.moment.duration.fn.toString)
- description and source-code
```javascript
function toISOString$1() {
    // for ISO strings we do not use the normal bubbling rules:
    //  * milliseconds bubble up until they become hours
    //  * days do not bubble at all
    //  * months bubble up until they become years
    // This is because there is no context-free conversion between hours and days
    // (think of clock changes)
    // and also not between days and months (28-31 days per month)
    if (!this.isValid()) {
        return this.localeData().invalidDate();
    }

    var seconds = abs$1(this._milliseconds) / 1000;
    var days         = abs$1(this._days);
    var months       = abs$1(this._months);
    var minutes, hours, years;

    // 3600 seconds -> 60 minutes -> 1 hour
    minutes           = absFloor(seconds / 60);
    hours             = absFloor(minutes / 60);
    seconds %= 60;
    minutes %= 60;

    // 12 months -> 1 year
    years  = absFloor(months / 12);
    months %= 12;


    // inspired by https://github.com/dordille/moment-isoduration/blob/master/moment.isoduration.js
    var Y = years;
    var M = months;
    var D = days;
    var h = hours;
    var m = minutes;
    var s = seconds;
    var total = this.asSeconds();

    if (!total) {
        // this is the same as C#'s (Noda) and python (isodate)...
        // but not other JS (goog.date)
        return 'P0D';
    }

    return (total < 0 ? '-' : '') +
        'P' +
        (Y ? Y + 'Y' : '') +
        (M ? M + 'M' : '') +
        (D ? D + 'D' : '') +
        ((h || m || s) ? 'T' : '') +
        (h ? h + 'H' : '') +
        (m ? m + 'M' : '') +
        (s ? s + 'S' : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.valueOf"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>valueOf ()](#apidoc.element.moment.duration.fn.valueOf)
- description and source-code
```javascript
function valueOf$1() {
    if (!this.isValid()) {
        return NaN;
    }
    return (
        this._milliseconds +
        this._days * 864e5 +
        (this._months % 12) * 2592e6 +
        toInt(this._months / 12) * 31536e6
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.weeks"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>weeks ()](#apidoc.element.moment.duration.fn.weeks)
- description and source-code
```javascript
function weeks() {
    return absFloor(this.days() / 7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment.duration.fn.years"></a>[function <span class="apidocSignatureSpan">moment.duration.fn.</span>years ()](#apidoc.element.moment.duration.fn.years)
- description and source-code
```javascript
years = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
