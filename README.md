# npmdoc-uglifyjs

#### api documentation for  [uglifyjs (v2.4.10)](http://lisperator.net/uglifyjs)  [![npm package](https://img.shields.io/npm/v/npmdoc-uglifyjs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-uglifyjs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-uglifyjs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-uglifyjs)

#### JavaScript parser, mangler/compressor and beautifier toolkit

[![NPM](https://nodei.co/npm/uglifyjs.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/uglifyjs)

- [https://npmdoc.github.io/node-npmdoc-uglifyjs/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-uglifyjs/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-uglifyjs/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-uglifyjs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-uglifyjs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-uglifyjs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bin": {
        "uglifyjs": "bin/uglifyjs"
    },
    "browserify": {
        "transform": [
            "uglify-to-browserify"
        ]
    },
    "bugs": {
        "url": "https://github.com/mishoo/UglifyJS2/issues"
    },
    "dependencies": {
        "async": "~0.2.6",
        "source-map": "0.1.34",
        "uglify-to-browserify": "~1.0.0",
        "yargs": "~1.3.3"
    },
    "description": "JavaScript parser, mangler/compressor and beautifier toolkit",
    "devDependencies": {
        "acorn": "~0.6.0",
        "escodegen": "~1.3.3",
        "esfuzz": "~0.3.1",
        "estraverse": "~1.5.1"
    },
    "directories": {},
    "dist": {
        "shasum": "632927319fa6a3da3fc91f9773ac27bfe6c3ee92",
        "tarball": "https://registry.npmjs.org/uglifyjs/-/uglifyjs-2.4.10.tgz"
    },
    "engines": {
        "node": ">=0.4.0"
    },
    "gitHead": "9de7199b88edb37753a36a9688d34a4be801f41b",
    "homepage": "http://lisperator.net/uglifyjs",
    "license": "BSD",
    "main": "tools/node.js",
    "maintainers": [
        {
            "name": "mytry"
        }
    ],
    "name": "uglifyjs",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mishoo/UglifyJS2.git"
    },
    "scripts": {
        "test": "node test/run-tests.js"
    },
    "version": "2.4.10"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
