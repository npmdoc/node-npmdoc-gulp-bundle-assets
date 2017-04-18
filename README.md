# npmdoc-gulp-bundle-assets

#### api documentation for  [gulp-bundle-assets (v2.28.0)](https://github.com/dowjones/gulp-bundle-assets#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-bundle-assets.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-bundle-assets) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-bundle-assets.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-bundle-assets)

#### Create asset (js, css) bundles from a config file leveraging the power of streams

[![NPM](https://nodei.co/npm/gulp-bundle-assets.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/gulp-bundle-assets)

- [https://npmdoc.github.io/node-npmdoc-gulp-bundle-assets/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-gulp-bundle-assets/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-bundle-assets/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-bundle-assets/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-bundle-assets/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-bundle-assets/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Montgomery",
        "url": "http://www.chrismontgomery.info/"
    },
    "bugs": {
        "url": "https://github.com/dowjones/gulp-bundle-assets/issues"
    },
    "contributors": [
        {
            "name": "Chris Montgomery",
            "url": "http://www.chrismontgomery.info/"
        },
        {
            "name": "Christian Sherland",
            "url": "https://github.com/csherland"
        },
        {
            "name": "Roberto Soares",
            "url": "https://github.com/roberto"
        },
        {
            "name": "bas",
            "url": "https://github.com/21brains-zh"
        },
        {
            "name": "gregorymaertens",
            "url": "https://github.com/gregorymaertens"
        },
        {
            "name": "narthollis",
            "url": "https://github.com/narthollis"
        },
        {
            "name": "PlasmaPower",
            "url": "https://github.com/PlasmaPower"
        }
    ],
    "dependencies": {
        "bluebird": "3.3.5",
        "duplexer2": "0.0.2",
        "graceful-fs": "4.1.4",
        "gulp": "3.9.1",
        "gulp-clean-css": "2.0.7",
        "gulp-coffee": "2.3.2",
        "gulp-concat": "2.5.2",
        "gulp-if": "2.0.1",
        "gulp-less": "3.1.0",
        "gulp-order": "1.1.1",
        "gulp-rev": "4.0.0",
        "gulp-sourcemaps": "1.5.2",
        "gulp-streamify": "0.0.5",
        "gulp-uglify": "1.5.3",
        "gulp-util": "3.0.7",
        "lazypipe": "0.2.3",
        "lodash": "3.9.3",
        "map-stream": "0.0.6",
        "merge-stream": "0.1.7",
        "mkdirp": "0.5.1",
        "pretty-hrtime": "1.0.2",
        "readable-stream": "2.0.0",
        "through2": "2.0.1",
        "vinyl": "1.1.1"
    },
    "description": "Create asset (js, css) bundles from a config file leveraging the power of streams",
    "devDependencies": {
        "browserify": "10.2.4",
        "coveralls": "2.11.2",
        "gulp-help": "1.6.0",
        "gulp-istanbul": "0.10.0",
        "gulp-istanbul-enforcer": "1.0.3",
        "gulp-jshint": "1.11.0",
        "gulp-mocha": "2.1.1",
        "gulp-nice-package": "1.0.0",
        "gulp-sass": "2.0.4",
        "gulp-shrinkwrap": "2.0.1",
        "jshint-stylish": "2.0.0",
        "mocha-lcov-reporter": "0.0.2",
        "multiline": "1.0.2",
        "proxyquire": "1.5.0",
        "rimraf": "^2.5.2",
        "should": "6.0.3",
        "sinon": "1.15.3",
        "vinyl-source-stream": "1.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "ee770e85e66cccb064568d92f1987d252c218f69",
        "tarball": "https://registry.npmjs.org/gulp-bundle-assets/-/gulp-bundle-assets-2.28.0.tgz"
    },
    "gitHead": "6cd1bdb4064aed7c8b5d92b4e8029ed85cef5e82",
    "homepage": "https://github.com/dowjones/gulp-bundle-assets#readme",
    "keywords": [
        "gulp",
        "gulpfriendly",
        "bundle",
        "bundles",
        "bundling",
        "assets",
        "asset",
        "combine",
        "compress",
        "minify",
        "minification",
        "package",
        "static",
        "resource",
        "javascript",
        "css"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "chmontgomery"
        }
    ],
    "name": "gulp-bundle-assets",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/dowjones/gulp-bundle-assets.git"
    },
    "scripts": {
        "coveralls": "gulp test-cover && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js && rm -rf ./coverage",
        "test": "gulp ci"
    },
    "version": "2.28.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
