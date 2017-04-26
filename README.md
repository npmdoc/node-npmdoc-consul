# npmdoc-consul

#### basic api documentation for  [consul (v0.28.0)](https://github.com/silas/node-consul#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-consul.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-consul) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-consul.svg)](https://travis-ci.org/npmdoc/node-npmdoc-consul)

#### Consul client

[![NPM](https://nodei.co/npm/consul.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/consul)

- [https://npmdoc.github.io/node-npmdoc-consul/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-consul/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-consul/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-consul/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-consul/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-consul/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Silas Sewell"
    },
    "bugs": {
        "url": "https://github.com/silas/node-consul/issues"
    },
    "dependencies": {
        "papi": "^0.27.0"
    },
    "description": "Consul client",
    "devDependencies": {
        "async": "^1.4.0",
        "bluebird": "^3.1.1",
        "debug": "^2.1.3",
        "istanbul": "^0.3.8",
        "jscs": "^2.1.1",
        "jshint": "^2.5.5",
        "lodash": "^3.5.0",
        "mocha": "^2.2.1",
        "nock": "^2.9.1",
        "node-uuid": "^1.4.3",
        "should": "^7.0.2",
        "sinon": "^1.14.1",
        "temp": "^0.8.1"
    },
    "directories": {},
    "dist": {
        "shasum": "c478fe6c58b6154b72867ef57ca8cfac181fba92",
        "tarball": "https://registry.npmjs.org/consul/-/consul-0.28.0.tgz"
    },
    "gitHead": "a0726641a976a8c93bac67754a764bc90642eab3",
    "homepage": "https://github.com/silas/node-consul#readme",
    "keywords": [
        "consul"
    ],
    "license": "MIT",
    "main": "./lib",
    "maintainers": [
        {
            "name": "silas"
        }
    ],
    "name": "consul",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/silas/node-consul.git"
    },
    "scripts": {
        "acceptance": "ACCEPTANCE=true istanbul cover --report text _mocha -- test/acceptance --recursive --check-leaks --timeout 15000",
        "cover": "istanbul cover _mocha -- --recursive && open coverage/lcov-report/index.html",
        "test": "jshint lib test && jscs lib test && istanbul cover --report text _mocha -- --recursive --check-leaks && istanbul check-coverage --statements 100 --functions 100 --branches 100 --lines 100"
    },
    "version": "0.28.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
