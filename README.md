# npmdoc-fs-extra-promise

#### api documentation for  fs-extra-promise (v1.0.1)  [![npm package](https://img.shields.io/npm/v/npmdoc-fs-extra-promise.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fs-extra-promise) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fs-extra-promise.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fs-extra-promise)

#### Node file system library and fs-extra module promisified with bluebird

[![NPM](https://nodei.co/npm/fs-extra-promise.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/fs-extra-promise)

- [https://npmdoc.github.io/node-npmdoc-fs-extra-promise/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-fs-extra-promise/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fs-extra-promise/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fs-extra-promise/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fs-extra-promise/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fs-extra-promise/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "fs-extra-promise",
    "version": "1.0.1",
    "description": "Node file system library and fs-extra module promisified with bluebird",
    "main": "./lib/",
    "author": {
        "name": "Overlook Motel"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/overlookmotel/fs-extra-promise.git"
    },
    "bugs": {
        "url": "https://github.com/overlookmotel/fs-extra-promise/issues"
    },
    "dependencies": {
        "fs-extra": "^2.1.2",
        "bluebird": "^3.5.0"
    },
    "devDependencies": {
        "mocha": "^3.2.0",
        "chai": "^3.5.0",
        "chai-as-promised": "^6.0.0",
        "jshint": "^2.9.4",
        "istanbul": "^0.4.5",
        "coveralls": "^2.13.0"
    },
    "keywords": [
        "fs",
        "fs-extra",
        "file",
        "promise",
        "bluebird",
        "extend"
    ],
    "scripts": {
        "test": "if [ $COVERAGE ]; then npm run coveralls; else npm run jshint && npm run test-main; fi",
        "jshint": "./node_modules/.bin/jshint lib test",
        "test-main": "./node_modules/mocha/bin/mocha --check-leaks --colors -t 10000 --reporter spec 'test/**/*.test.js'",
        "cover": "npm run cover-main && rm -rf coverage",
        "coveralls": "npm run cover-main && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js && rm -rf ./coverage",
        "cover-main": "COVERAGE=true ./node_modules/.bin/istanbul cover ./node_modules/.bin/_mocha --report lcovonly -- -R spec 'test/**/*.test.js'"
    },
    "engines": {
        "node": ">=4"
    },
    "readmeFilename": "README.md",
    "license": "MIT"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
