# eslint-config-vue2

A configuration of ESLint for Vue 2.x

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
