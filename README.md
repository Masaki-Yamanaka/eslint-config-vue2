# eslint-config-vue2

Configuration of ESLint for Vue 2.x

## Usage

```bash
# Install dependencies
yarn add -D babel-eslint eslint eslint-config-airbnb-base eslint-config-prettier eslint-plugin-import eslint-plugin-vue
```

- Copy .eslintrc.js .eslintignore
- Add following scripts in package.json

```bash
"scripts": {
  "lint:js": "eslint . --ext .js,.vue",
  "lint:js:fix": "eslint . --ext .js,.vue --fix"
}
```

### Prettier

Since turned off all rules that might conflict with Prettier, please make sure Prettier is installed.

```bash
# Install dependencies
yarn add -D prettier
```

- Add following scripts in package.json

```bash
"scripts": {
  "format:js": "prettier -c (directory)",
  "format:js:fix": "prettier -w (directory)"
}
```

### jQuery
If you use jQuery, you must install eslint-plugin-jquery and add following in .eslintrc.js
```bash
# Install dependencies
yarn add -D eslint-plugin-jquery
```
```bash
module.exports = {
  env: {
    jquery: true
  },
  plugins: ["jquery"]
}
```
