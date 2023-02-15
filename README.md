# vue-pug-indent-reproduction

## Steps to reproduce

- `npm install`
- `npm run dev`
- Open in browser.
- Observe error in terminal:

```
unexpected token "indent"
  Plugin: vite:vue
  File: …/vue-pug-indent-reproduction/src/App.vue
      at makeError (…/vue-pug-indent-reproduction/node_modules/pug-error/index.js:34:13)
      at Parser.error (…/vue-pug-indent-reproduction/node_modules/pug-parser/index.js:56:15)
      at Parser.parseExpr (…/vue-pug-indent-reproduction/node_modules/pug-parser/index.js:280:14)
      at Parser.parse (…/vue-pug-indent-reproduction/node_modules/pug-parser/index.js:115:25)
      at parse (…/vue-pug-indent-reproduction/node_modules/pug-parser/index.js:12:20)
      at Object.parse (…/vue-pug-indent-reproduction/node_modules/pug/lib/index.js:137:11)
      at Function.loadString [as string] (…/vue-pug-indent-reproduction/node_modules/pug-load/index.js:54:21)
      at compileBody (…/vue-pug-indent-reproduction/node_modules/pug/lib/index.js:82:18)
      at Object.exports.compile (…/vue-pug-indent-reproduction/node_modules/pug/lib/index.js:269:16)
      at …/vue-pug-indent-reproduction/node_modules/@vue/compiler-sfc/dist/compiler-sfc.cjs.js:2382:59
```

## Related

- https://github.com/vuejs/core/pull/7723
- https://github.com/vuejs/core/pull/3842
- https://github.com/vuejs/core/issues/3231
- https://github.com/yyx990803/pug-plain-loader/issues/18
