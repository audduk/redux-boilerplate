React-redux boilerplate
=======================
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com/)
![](https://img.shields.io/badge/version-0.0.1-green.svg)

Features
--------
* Webpack build with JSX syntax and ES2015
* React and Redux
* Redux router
* Redux dev tools and hot reload
* Tests with *Jest* and **React Test Utilities** (There is an [issue](https://github.com/facebook/react/issues/4972) with stateless components testing)
* **Standard.js** code styles checks
* Less preprocessor with autoprefixer
* Bootstrap

Commands
--------
* `npm start` - start webpack development server with hot reload and dev-tools
* `npm run build` - build for production
* `npm run lint` - check code style
* `npm run jest` - run tests
* `npm run test` - check code style and run tests
* `npm run clean` - remove build results
* `npm run package` - runs tests, builds project for production and creates tarball ready for deployment to webserver root
**Note**
Some commands will run on both unix and windows, but most work only Mac and Linux.

Gotchas
-------
* There is some magic done by **Jest** and **TestUtils**. jest.dontMock('path') does not work with es6 import sometimes. **USE require('path') in jest tests** while testing components.
* Stateless(arrow) components cannot be tested with test utils(yet) cause of [this issue](https://github.com/facebook/react/issues/4972)
