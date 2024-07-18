# Setup

Below are the steps to setup and create new repo

- [Setup](#setup)
- [Initialize this repo](#initialize-this-repo)
- [Add bootstrap 5](#add-bootstrap-5)
- [Deploy vue.js app on github pages](#deploy-vuejs-app-on-github-pages)
  - [Deployment using gh-pages](#deployment-using-gh-pages)


# Initialize this repo

- [markdown basic syntax](https://www.markdownguide.org/basic-syntax){:target="\_blank"}
- Install nvm [node version manager](https://github.com/nvm-sh/nvm?tab=readme-ov-file#install--update-script){:target="\_blank"}
- nvm

```shell
nvm --version # current installed nvm version
nvm --help    # help options
```

- node version

```shell
nvm ls-remote               # list of remote node versions
nvm ls-remote --lts
nvm install --lts --default # install lts version and make it default
nvm use v20.15.1            # use new --lts version just installed
nvm current                 # current used node version
npm --version               # version of npm
nvm install-latest-npm      # latest npm for current node version
node --version > .nvmrc     # create or update .nvmrc
nvm use                     # user version from .nvmrc
```

- creating new vue-js-3 app using [quickstart](https://vuejs.org/guide/quick-start.html){:target="\_blank"}
  - `npm create vue@latest` OR
  - `npm init vue@latest` OR
  - `npm init vite@latest`, and then select `vue`.

# Add bootstrap 5

- install dependencies

```sh
npm i bootstrap @popperjs/core bootstrap-icons
npm i sass --save-dev
./node_modules/.bin/sass --version
```

- `assets/scss/styles.scss` : create this file and import bootstrap css as below

```scss
// Import Bootstrap
@import 'bootstrap/scss/bootstrap';

// Import Bootstrap Icons w/ custom path to fonts folder
$bootstrap-icons-font-dir: 'bootstrap-icons/font/fonts';
@import 'bootstrap-icons/font/bootstrap-icons';

// Custom styles
body {
  padding: 1.5rem;
  margin: 1rem;
  border: solid red 1px;
}
```

- `main.css` : import `styles.scss` at the top of file

```js
@import './scss/styles.scss';
```

- `main.js` : imports bootstrap js bundle after `main.css` import

```js
// import bootstrap js
import 'bootstrap/dist/js/bootstrap.bundle'
```

# Deploy vue.js app on github pages

For this repo we use `gh-pages` branch to host on github pages.

we use gh-pages library to push changes to branch.

## Deployment using gh-pages

- `vite.config.ts` - add attribute base for path to repository.
- `package.json`
  - add `gh-pages` dependency and
  - `deploy` script.

```sh
# vite.config.ts
base: "/learn-vue-js/",

# install command to add as dev dependencies
npm i gh-pages --save-dev
./node_modules/.bin/gh-pages --version

# package.json
"deploy": "npm run build && gh-pages -d dist"
```

- Run `npm run deploy` from terminal, this creates a dist folder and commits it to branch gh-pages on github.
- gh pages deploy from branch `gh-pages`.
