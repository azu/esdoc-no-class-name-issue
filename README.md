# esdoc-no-class-name-issue

[ESDoc](https://github.com/h13i32maru/esdoc "ESDoc") has anonymous class issue.

```js
// anonymous class
export default class {
    constructor(){
        this.description = "this is example class";
    }
}
```

## Installation

    npm install

## Issue

```sh
$ npm run doc

> esdoc-no-class-name-issue@1.0.0 doc /Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue
> esdoc -c esdoc.json

/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/ESDoc.js:378
            throw _iteratorError5;
                  ^
TypeError: Cannot read property 'name' of null
    at ClassDoc.name (/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/Doc/ClassDoc.js:70:39)
    at ClassDoc._apply (/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/Doc/AbstractDoc.js:68:20)
    at ClassDoc._apply (/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/Doc/ClassDoc.js:48:71)
    at ClassDoc.AbstractDoc (/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/Doc/AbstractDoc.js:54:10)
    at new ClassDoc (/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/Doc/ClassDoc.js:34:20)
    at DocFactory._createDoc (/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/Factory/DocFactory.js:388:14)
    at DocFactory._traverseComments (/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/Factory/DocFactory.js:318:24)
    at DocFactory.push (/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/Factory/DocFactory.js:206:26)
    at Controller.<anonymous> (/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/ESDoc.js:411:17)
    at Controller.enter (/Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/node_modules/esdoc/out/src/Util/ASTUtil.js:42:20)

npm ERR! Darwin 14.3.0
npm ERR! argv "node" "/Users/azu/.nodebrew/current/bin/npm" "run" "doc"
npm ERR! node v0.12.0
npm ERR! npm  v2.9.0
npm ERR! code ELIFECYCLE
npm ERR! esdoc-no-class-name-issue@1.0.0 doc: `esdoc -c esdoc.json`
npm ERR! Exit status 1
npm ERR!
npm ERR! Failed at the esdoc-no-class-name-issue@1.0.0 doc script 'esdoc -c esdoc.json'.
npm ERR! This is most likely a problem with the esdoc-no-class-name-issue package,
npm ERR! not with npm itself.
npm ERR! Tell the author that this fails on your system:
npm ERR!     esdoc -c esdoc.json
npm ERR! You can get their info via:
npm ERR!     npm owner ls esdoc-no-class-name-issue
npm ERR! There is likely additional logging output above.

npm ERR! Please include the following file with any support request:
npm ERR!     /Users/azu/.ghq/github.com/azu/esdoc-no-class-name-issue/npm-debug.log
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

MIT