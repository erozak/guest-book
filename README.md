# Guest Book

> [!WARNING]
> This repository is archived. It is no longer maintained and will not receive updates.

A small guest book app built with Vue.js. Visitors can leave a short message with a nickname, gender icon and optional contact email, and read the messages left by others.

## Features

- Message editor with validation (nickname: letters and spaces, max 56 chars; email format; message: required, max 140 chars)
- Toggleable editor panel
- Message list with relative timestamps that refresh over time
- State managed with Vuex (`book` and `frame` modules)

## Tech Stack

- [Vue 2](https://vuejs.org/), [Vue Router](https://router.vuejs.org/), [Vuex](https://vuex.vuejs.org/)
- [vee-validate](https://baianat.github.io/vee-validate/) for form validation
- Pug and SCSS for templates and styles
- Webpack 3, Babel, ESLint (airbnb-base)
- Karma / Mocha / Sinon-Chai for unit tests, Nightwatch for e2e tests

## Getting Started

``` bash
# install dependencies
yarn install

# serve with hot reload at localhost:8080
yarn dev

# build for production with minification
yarn build

# run unit tests
yarn unit

# run e2e tests
yarn e2e

# run all tests
yarn test

# lint sources and specs
yarn lint
```

## Project Structure

```
src/
├── components/   Book, Editor, EditorToggler, Message
├── frame/        Header, Footer
├── router/       Vue Router setup
├── store/        Vuex store (modules: book, frame)
├── styles/       Shared SCSS (variables, utils, components)
├── App.vue
└── main.js
```

## Author

Erozak &lt;pinex666@gmail.com&gt;
