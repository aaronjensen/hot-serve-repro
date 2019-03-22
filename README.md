Repro for https://github.com/shellscape/webpack-plugin-serve/issues/117

To start:

```sh
yarn
yarn wp --watch --config config/webpack.config.js
```

open https://localhost:3000

These are the errors I see:

```
react-dom.development.js:2490 Uncaught TypeError: Cannot read property 'hasOwnProperty' of undefined
    at react-dom.development.js:2490
    at Object../node_modules/react-dom/cjs/react-dom.development.js (react-dom.development.js:22346)
    at __webpack_require__ (bootstrap:781)
    at fn (bootstrap:149)
    at Object../node_modules/react-dom/index.js (index.js:36)
    at __webpack_require__ (bootstrap:781)
    at fn (bootstrap:149)
    at Object../node_modules/react-hot-loader/dist/react-hot-loader.development.js (react-hot-loader.development.js:17)
    at __webpack_require__ (bootstrap:781)
    at fn (bootstrap:149)
(anonymous) @ react-dom.development.js:2490
./node_modules/react-dom/cjs/react-dom.development.js @ react-dom.development.js:22346
__webpack_require__ @ bootstrap:781
fn @ bootstrap:149
./node_modules/react-dom/index.js @ index.js:36
__webpack_require__ @ bootstrap:781
fn @ bootstrap:149
./node_modules/react-hot-loader/dist/react-hot-loader.development.js @ react-hot-loader.development.js:17
__webpack_require__ @ bootstrap:781
fn @ bootstrap:149
./node_modules/react-hot-loader/index.js @ index.js:23
__webpack_require__ @ bootstrap:781
fn @ bootstrap:149
register @ index.js:101
./node_modules/object-assign/index.js @ index.js:135
__webpack_require__ @ bootstrap:781
fn @ bootstrap:149
(anonymous) @ react.development.js:15
./node_modules/react/cjs/react.development.js @ react.development.js:1920
__webpack_require__ @ bootstrap:781
fn @ bootstrap:149
./node_modules/react/index.js @ index.js:6
__webpack_require__ @ bootstrap:781
fn @ bootstrap:149
./src/index.js @ index.css?02e3:45
__webpack_require__ @ bootstrap:781
fn @ bootstrap:149
0 @ serviceWorker.js:129
__webpack_require__ @ bootstrap:781
checkDeferredModules @ bootstrap:45
webpackJsonpCallback @ bootstrap:32
(anonymous) @ main.chunk.js:1
Show 2 more frames
manifest.json:1 GET http://localhost:3000/manifest.json 404 (Not Found)
manifest.json:1 Manifest: Line: 1, column: 1, Unexpected token.
```
