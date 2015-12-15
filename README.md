# PostHTML-bemjson

[![Join the chat at https://gitter.im/theprotein/posthtml-bemjson](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/theprotein/posthtml-bemjson?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![npm version](https://badge.fury.io/js/posthtml-bemjson.svg)](http://badge.fury.io/js/posthtml-bemjson)

[PostHTML](https://github.com/posthtml/posthtml) plugin to convert PostHTML tree to [BEMJSON](https://en.bem.info/technology/bemjson/) tree

## Usage

```js
var posthtml = require('posthtml'),
    html = '<html><head><title>Wow</title></head><body><div class="button"><div class="button__text">Text</div></div></body></html>';

var bemjson = posthtml()
    .use(require('posthtml-bemjson'))
    .process(html, { sync: true }).tree;
```

## Test

```
npm run test
```

