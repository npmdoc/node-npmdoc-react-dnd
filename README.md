# npmdoc-react-dnd

#### basic api documentation for  react-dnd (v2.3.0)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-dnd.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-dnd) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-dnd.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-dnd)

#### Drag and Drop for React

[![NPM](https://nodei.co/npm/react-dnd.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-dnd)

- [https://npmdoc.github.io/node-npmdoc-react-dnd/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-dnd/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-dnd/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-dnd/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-dnd/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-dnd/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "dependencies": {
        "disposables": "^1.0.1",
        "dnd-core": "^2.3.0",
        "hoist-non-react-statics": "^1.2.0",
        "invariant": "^2.1.0",
        "lodash": "^4.2.0"
    },
    "description": "Drag and Drop for React",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "aede61c06b968554dcf2a2445657cdbb3100be49",
        "tarball": "https://registry.npmjs.org/react-dnd/-/react-dnd-2.3.0.tgz"
    },
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "darthtrevino"
        },
        {
            "name": "gaearon"
        },
        {
            "name": "jordangens"
        }
    ],
    "name": "react-dnd",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0-0"
    },
    "scripts": {
        "babel": "../../node_modules/.bin/babel src --out-dir lib",
        "build": "../../node_modules/.bin/npm-run-all --parallel bundle:* babel",
        "bundle:min": "../../node_modules/.bin/webpack --output-filename=dist/ReactDnD.min.js --optimize-minimize",
        "bundle:unmin": "../../node_modules/.bin/webpack --output-filename=dist/ReactDnD.js",
        "clean": "../../node_modules/.bin/rimraf lib dist",
        "prepublish": "npm test",
        "test": "../../node_modules/.bin/npm-run-all clean build"
    },
    "version": "2.3.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
