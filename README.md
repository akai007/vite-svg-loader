# Vite SVG loader
Vite 2.x plugin to load SVG files as Vue components.

<a href="https://www.npmjs.com/package/vite-svg-loader" target="_blank"><img src="https://img.shields.io/npm/v/vite-svg-loader?style=flat-square" alt="Version"></a>
<a href="https://www.npmjs.com/package/vite-svg-loader" target="_blank"><img src="https://img.shields.io/npm/l/vite-svg-loader?style=flat-square" alt="License"></a>

```vue
<template>
  <MyIcon />
</template>

<script setup>
import MyIcon from './my-icon.svg'
</script>
```

### Install
```bash
npm install vite-svg-loader --save-dev
```

### Setup

#### `vite.config.js`
```js
import svgLoader from 'vite-svg-loader'

export default {
  plugins: [vue(), svgLoader()]
}
```

### Use with TypeScript
If you'd like to use the loader in a TypeScript project, you'll need to add the following type definition to your `tsconfig.json` file:

#### `tsconfig.json`
```json
{
  "compilerOptions": {
    "types": ["vite-svg-loader", "vite/client"]
  }
}
```
