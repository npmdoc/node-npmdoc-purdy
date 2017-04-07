# api documentation for  [purdy (v2.2.1)](https://github.com/danielb2/purdy.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-purdy.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-purdy) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-purdy.svg)](https://travis-ci.org/npmdoc/node-npmdoc-purdy)
#### Pretty print objects in real purdy colors. Allows clearer visualization of objects than you get from most pretty printers due to colors. It will also print out the complete path to an object, something that's extremly useful for debugging. Purdy will also

[![NPM](https://nodei.co/npm/purdy.png?downloads=true)](https://www.npmjs.com/package/purdy)

[![apidoc](https://npmdoc.github.io/node-npmdoc-purdy/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-purdy_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-purdy/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-purdy/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-purdy/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Daniel Bretoi"
    },
    "bin": {
        "purdy": "bin/purdy.js"
    },
    "bugs": {
        "url": "https://github.com/danielb2/purdy.js/issues"
    },
    "dependencies": {
        "chalk": "0.4.x",
        "hoek": "2.x.x",
        "joi": "6.x.x"
    },
    "description": "Pretty print objects in real purdy colors. Allows clearer visualization of objects than you get from most pretty printers due to colors. It will also print out the complete path to an object, something that's extremly useful for debugging. Purdy will also",
    "devDependencies": {
        "code": "1.x.x",
        "lab": "6.x.x"
    },
    "directories": {},
    "dist": {
        "shasum": "76787564da04f8ef7e9672987bf1d21a726699c4",
        "tarball": "https://registry.npmjs.org/purdy/-/purdy-2.2.1.tgz"
    },
    "gitHead": "b7bb68fc7ce56ceb71c3172c269848a34ac7f735",
    "homepage": "https://github.com/danielb2/purdy.js",
    "keywords": [
        "ansi",
        "terminal",
        "colors",
        "pretty",
        "print",
        "color"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "danielb",
            "email": "nefar@otherware.org"
        }
    ],
    "name": "purdy",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/danielb2/purdy.js.git"
    },
    "scripts": {
        "test": "lab -a code -t 100 -v -I Reflect"
    },
    "version": "2.2.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module purdy](#apidoc.module.purdy)
1.  [function <span class="apidocSignatureSpan">purdy.</span>stringify (object, options)](#apidoc.element.purdy.stringify)



# <a name="apidoc.module.purdy"></a>[module purdy](#apidoc.module.purdy)

#### <a name="apidoc.element.purdy.stringify"></a>[function <span class="apidocSignatureSpan">purdy.</span>stringify (object, options)](#apidoc.element.purdy.stringify)
- description and source-code
```javascript
stringify = function (object, options) {

    const Purdy = new internals.purdy(object, options);
    return Purdy.stringify();
}
```
- example usage
```shell
...
    * 'pathPrefix' - prefix for path. default: '// '
    * 'arrayIndex' - enables index printing for arrays. default: 'true'
    * 'indent' - defines the number of spaces to indent default: '4'
    * 'align' - determines how to align object keys. default: 'left'
    * 'depth' - tells purdy how many times to recurse while formatting the object. This is useful for viewing complicated objects
. default: '2'. Set to 'null' to recurse indefinitely


### 'Purdy.stringify(object, [options])'

This function returns a string without printing it to stdout. This may prove
to be useful for log files other other applications.

''' javascript
const purdyString = Purdy.stringify({a: 'b'}, {plain: true});
writeLog(purdyString);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
