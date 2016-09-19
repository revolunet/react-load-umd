# LoadUmd [![experimental](http://badges.github.io/stability-badges/dist/experimental.svg)](http://github.com/badges/stability-badges)

Async load any remote [UMD](https://github.com/umdjs/umd) compatible React component into your app.

This component use [script.js](https://github.com/ded/script.js/) for loading the remote component.

## Usage

You can use [unpkg.com](unpkg.com) or whatever hosting. The only requirement is that the build supports [UMD](https://github.com/umdjs/umd).

```js
import LoadUmd from 'react-load-umd'

let cmp = (<LoadUmd url="https://npmcdn.com/react-json-viewer@1.0.9" name="ReactJSONViewer" props={ props }>
             <p>Loading remote component...</p>
           </LoadUmd>);

```

As UMD exposes objects on `window`, you also need to define the name of the final module.


## Dev

This project use the great [react-component-boilerplate](https://github.com/survivejs/react-component-boilerplate)

