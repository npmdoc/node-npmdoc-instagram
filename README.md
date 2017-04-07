# api documentation for  [instagram (v0.0.4)](https://github.com/Swizec/nodestagram)  [![npm package](https://img.shields.io/npm/v/npmdoc-instagram.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-instagram) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-instagram.svg)](https://travis-ci.org/npmdoc/node-npmdoc-instagram)
#### Instagram API wrapper for node.

[![NPM](https://nodei.co/npm/instagram.png?downloads=true)](https://www.npmjs.com/package/instagram)

[![apidoc](https://npmdoc.github.io/node-npmdoc-instagram/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-instagram_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-instagram/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-instagram/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-instagram/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Swizec",
        "email": "swizec@swizec.com",
        "url": "http://swizec.com"
    },
    "bugs": {
        "url": "https://github.com/Swizec/nodestagram/issues"
    },
    "dependencies": {},
    "description": "Instagram API wrapper for node.",
    "devDependencies": {},
    "directories": {
        "lib": "."
    },
    "dist": {
        "shasum": "ed49e921279330267cb1d98ff1bd59187af8791b",
        "tarball": "https://registry.npmjs.org/instagram/-/instagram-0.0.4.tgz"
    },
    "engines": {
        "node": "*"
    },
    "files": [],
    "homepage": "https://github.com/Swizec/nodestagram",
    "main": "./index.js",
    "name": "instagram",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/Swizec/nodestagram.git"
    },
    "version": "0.0.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module instagram](#apidoc.module.instagram)
1.  [function <span class="apidocSignatureSpan">instagram.</span>createClient (client_id, client_secret)](#apidoc.element.instagram.createClient)



# <a name="apidoc.module.instagram"></a>[module instagram](#apidoc.module.instagram)

#### <a name="apidoc.element.instagram.createClient"></a>[function <span class="apidocSignatureSpan">instagram.</span>createClient (client_id, client_secret)](#apidoc.element.instagram.createClient)
- description and source-code
```javascript
createClient = function (client_id, client_secret) {
    var instagram_client = new InstagramClient(client_id, client_secret);

    return instagram_client;
}
```
- example usage
```shell
...

The convention being that when the error is null, the result contains media as returnd from the API,
and when something goes wrong error is the status code as returned by the API and the result is the
meta info the API returned.

For example:

var instagram = require('instagram').createClient('<client_id>', '<client_secret>');

// fetch media by id
instagram.media.id('<id>', function (images, error) { ... });

// fetch popular media
instagram.media.popular(function (images, error) { ... });
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
