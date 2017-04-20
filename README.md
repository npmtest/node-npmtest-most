# npmtest-most

#### basic test coverage for  most (v1.2.2)  [![npm package](https://img.shields.io/npm/v/npmtest-most.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-most) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-most.svg)](https://travis-ci.org/npmtest/node-npmtest-most)

#### Monadic streams

[![NPM](https://nodei.co/npm/most.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/most)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-most/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-most/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-most/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-most/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-most/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-most/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-most/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-most/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-most/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-most/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-most/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-most/build/test-report.html](https://npmtest.github.io/node-npmtest-most/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-most/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-most/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-most/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-most/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-most/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-most/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-most/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-most/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "most",
    "version": "1.2.2",
    "description": "Monadic streams",
    "typings": "type-definitions/most.d.ts",
    "main": "lib/index.js",
    "module": "src/index.js",
    "jsnext:main": "src/index.js",
    "files": [
        "src",
        "lib",
        "type-definitions",
        "dist"
    ],
    "scripts": {
        "unit-test": "buster-test",
        "test": "eslint src test && npm run unit-test && npm run doctest",
        "build": "rimraf lib dist && buba src -o lib && rollup -c && uglifyjs dist/most.js -c \"warnings=false\" -m -o dist/most.min.js",
        "preversion": "npm run build",
        "doctest": "markdown-doctest"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/cujojs/most"
    },
    "keywords": [
        "reactive",
        "reactive programming",
        "reactive streams",
        "stream",
        "streams",
        "event stream",
        "promise",
        "promises",
        "promises-aplus",
        "fantasy-land",
        "monad",
        "monadic",
        "functional",
        "async",
        "cujojs",
        "cujo"
    ],
    "author": "brian@hovercraftstudios.com",
    "license": "MIT",
    "devDependencies": {
        "@most/eslint-config-most": "^1.0.3",
        "@most/hold": "1.4.2",
        "babel-polyfill": "^6.20.0",
        "buba": "^4.0.1",
        "buster": "^0.7.18",
        "eslint": "^3.12.1",
        "markdown-doctest": "^0.9.1",
        "rimraf": "^2.5.4",
        "rollup": "^0.39.2",
        "rollup-plugin-buble": "^0.15.0",
        "rollup-plugin-node-resolve": "^2.0.0",
        "transducers-js": "^0.4.174",
        "uglify-js": "^2.7.5"
    },
    "dependencies": {
        "@most/multicast": "^1.2.5",
        "@most/prelude": "^1.4.0",
        "symbol-observable": "^1.0.2"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
