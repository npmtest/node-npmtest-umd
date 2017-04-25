# npmtest-umd

#### basic test coverage for  [umd (v3.0.1)](https://github.com/ForbesLindesay/umd)  [![npm package](https://img.shields.io/npm/v/npmtest-umd.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-umd) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-umd.svg)](https://travis-ci.org/npmtest/node-npmtest-umd)

#### Universal Module Definition for use in automated build systems

[![NPM](https://nodei.co/npm/umd.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/umd)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-umd/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-umd/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-umd/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-umd/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-umd/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-umd/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-umd/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-umd/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-umd/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-umd/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-umd/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-umd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-umd/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-umd/build/test-report.html](https://npmtest.github.io/node-npmtest-umd/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-umd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-umd/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-umd/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-umd/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-umd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-umd/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-umd/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-umd/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "ForbesLindesay"
    },
    "bin": {
        "umd": "./bin/cli.js"
    },
    "bugs": {
        "url": "https://github.com/ForbesLindesay/umd/issues"
    },
    "dependencies": {},
    "description": "Universal Module Definition for use in automated build systems",
    "devDependencies": {
        "brfs": "^1.3.0",
        "linify": "~1.0.1",
        "mocha": "*",
        "uglify-js": "~2.4.0"
    },
    "directories": {},
    "dist": {
        "shasum": "8ae556e11011f63c2596708a8837259f01b3d60e",
        "tarball": "https://registry.npmjs.org/umd/-/umd-3.0.1.tgz"
    },
    "files": [
        "index.js",
        "bin/cli.js"
    ],
    "gitHead": "8fc39397901723d695136ee1fdceefb8e0392f5f",
    "homepage": "https://github.com/ForbesLindesay/umd",
    "license": "MIT",
    "maintainers": [
        {
            "name": "forbeslindesay"
        },
        {
            "name": "zertosh"
        },
        {
            "name": "jazz"
        },
        {
            "name": "ralphtheninja"
        }
    ],
    "name": "umd",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/ForbesLindesay/umd.git"
    },
    "scripts": {
        "build": "uglifyjs template.js > template.min.js && brfs source.js > index.js",
        "prepublish": "npm run build && linify transform bin",
        "test": "npm run build && mocha -R spec"
    },
    "version": "3.0.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
