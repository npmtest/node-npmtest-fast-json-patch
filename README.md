# npmtest-fast-json-patch

#### basic test coverage for  [fast-json-patch (v1.1.9)](https://github.com/Starcounter-Jack/JSON-Patch)  [![npm package](https://img.shields.io/npm/v/npmtest-fast-json-patch.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-fast-json-patch) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-fast-json-patch.svg)](https://travis-ci.org/npmtest/node-npmtest-fast-json-patch)

#### Fast implementation of JSON-Patch (RFC-6902) with duplex (observe changes) capabilities

[![NPM](https://nodei.co/npm/fast-json-patch.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/fast-json-patch)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-fast-json-patch/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-fast-json-patch/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-fast-json-patch/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-fast-json-patch/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-fast-json-patch/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-fast-json-patch/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-fast-json-patch/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-fast-json-patch/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-fast-json-patch/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-fast-json-patch/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-fast-json-patch/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-fast-json-patch/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-fast-json-patch/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-fast-json-patch/build/test-report.html](https://npmtest.github.io/node-npmtest-fast-json-patch/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-fast-json-patch/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-fast-json-patch/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-fast-json-patch/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-fast-json-patch/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fast-json-patch/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fast-json-patch/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-fast-json-patch/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-fast-json-patch/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Joachim Wester",
        "url": "http://www.starcounter.com/"
    },
    "bugs": {
        "url": "https://github.com/Starcounter-Jack/JSON-Patch/issues"
    },
    "dependencies": {},
    "description": "Fast implementation of JSON-Patch (RFC-6902) with duplex (observe changes) capabilities",
    "devDependencies": {
        "benchmark": "^2.1.2",
        "chalk": "^1.1.3",
        "grunt": "^0.4.5",
        "grunt-bump": "^0.3.0",
        "grunt-contrib-uglify": "~0.5.0",
        "jasmine": "^2.5.1",
        "jsdom": "^9.5.0",
        "jsonfile": "^2.3.1",
        "typescript": "~2.0.0",
        "underscore": "^1.8.3"
    },
    "directories": {},
    "dist": {
        "shasum": "1b3a864f838571b71d6a3aa7007287583b70cc5f",
        "tarball": "https://registry.npmjs.org/fast-json-patch/-/fast-json-patch-1.1.9.tgz"
    },
    "engines": {
        "node": ">= 0.4.0"
    },
    "gitHead": "fe07f88850af1ece9a1fc673198b233591258aac",
    "homepage": "https://github.com/Starcounter-Jack/JSON-Patch",
    "keywords": [
        "json",
        "patch",
        "http",
        "rest"
    ],
    "license": "MIT",
    "main": "src/json-patch-duplex.js",
    "maintainers": [
        {
            "name": "warpech"
        },
        {
            "name": "tomalec"
        }
    ],
    "name": "fast-json-patch",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/Starcounter-Jack/JSON-Patch.git"
    },
    "scripts": {
        "bench": "npm run bench-core && npm run bench-duplex",
        "bench-core": "node test/spec/coreBenchmark.js",
        "bench-duplex": "node test/spec/coreBenchmark.js DUPLEX=yes && node test/spec/duplexBenchmark.js",
        "bench-duplex-only": "node test/spec/duplexBenchmark.js",
        "test": "npm run test-core && npm run test-duplex",
        "test-core": "jasmine  DUPLEX=no JASMINE_CONFIG_PATH=test/jasmine.json test/spec/jsonPatchTestsSpec.js test/spec/coreSpec.js test/spec/validateSpec.js",
        "test-duplex": "jasmine DUPLEX=yes JASMINE_CONFIG_PATH=test/jasmine.json",
        "tsc": "tsc",
        "tsc-watch": "tsc -w",
        "uglify": "grunt uglify"
    },
    "typings": "src/json-patch-duplex.d.ts",
    "version": "1.1.9",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
