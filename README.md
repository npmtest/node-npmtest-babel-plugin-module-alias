# npmtest-babel-plugin-module-alias

#### basic test coverage for  [babel-plugin-module-alias (v1.6.0)](https://github.com/tleunen/babel-plugin-module-alias#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-babel-plugin-module-alias.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-babel-plugin-module-alias) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-babel-plugin-module-alias.svg)](https://travis-ci.org/npmtest/node-npmtest-babel-plugin-module-alias)

#### Babel plugin to rewrite the path in require() and ES6 import

[![NPM](https://nodei.co/npm/babel-plugin-module-alias.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/babel-plugin-module-alias)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-babel-plugin-module-alias/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-babel-plugin-module-alias/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/test-report.html](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-babel-plugin-module-alias/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-babel-plugin-module-alias/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-babel-plugin-module-alias/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-babel-plugin-module-alias/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-babel-plugin-module-alias/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tommy Leunen",
        "url": "http://tommyleunen.com"
    },
    "bugs": {
        "url": "https://github.com/tleunen/babel-plugin-module-alias/issues"
    },
    "dependencies": {},
    "deprecated": "WARNING: This project has been renamed to babel-plugin-module-resolver. Install babel-plugin-module-resolver for new features",
    "description": "Babel plugin to rewrite the path in require() and ES6 import",
    "devDependencies": {
        "babel-cli": "^6.10.1",
        "babel-core": "^6.8.0",
        "babel-plugin-__coverage__": "^11.0.0",
        "babel-preset-es2015": "^6.6.0",
        "babel-register": "^6.8.0",
        "condition-circle": "^1.2.0",
        "cross-env": "^1.0.8",
        "eslint": "^2.13.0",
        "eslint-config-airbnb-base": "^3.0.1",
        "eslint-plugin-import": "^1.9.1",
        "mocha": "^2.5.0",
        "nyc": "^6.6.1",
        "semantic-release": "^4.3.5"
    },
    "directories": {},
    "dist": {
        "shasum": "df7e3aaba3544f4c06a9d3314a26bbbff6d87b61",
        "tarball": "https://registry.npmjs.org/babel-plugin-module-alias/-/babel-plugin-module-alias-1.6.0.tgz"
    },
    "homepage": "https://github.com/tleunen/babel-plugin-module-alias#readme",
    "keywords": [
        "babel",
        "babel-plugin",
        "module",
        "alias",
        "rewrite",
        "resolve",
        "rename",
        "mapping",
        "require",
        "import"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "tleunen"
        }
    ],
    "name": "babel-plugin-module-alias",
    "nyc": {
        "sourceMap": false,
        "instrument": false,
        "reporter": [
            "lcov",
            "text"
        ]
    },
    "optionalDependencies": {},
    "release": {
        "verifyConditions": "condition-circle"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tleunen/babel-plugin-module-alias.git"
    },
    "scripts": {
        "compile": "cross-env NODE_ENV=production babel src --out-dir lib",
        "lint": "eslint src test",
        "prepublish": "npm run compile",
        "pretest": "npm run lint",
        "semantic-release": "semantic-release pre && npm publish && semantic-release post",
        "test": "cross-env NODE_ENV=test nyc npm run test:suite",
        "test:suite": "mocha --compilers js:babel-register",
        "test:watch": "npm run test:suite -- -w"
    },
    "version": "1.6.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
