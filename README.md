# learn-vue-js-3

Learning Vuej.js 3 with hands-on.
This template should help get you started developing with Vue 3 in Vite.

- [learn-vue-js-3](#learn-vue-js-3)
- [Recommended IDE Setup](#recommended-ide-setup)
  - [Customize configuration](#customize-configuration)
- [Project Setup](#project-setup)
- [Run localhost](#run-localhost)
    - [Sync checkout branch to latest chnages](#sync-checkout-branch-to-latest-chnages)
    - [Compile and Hot-Reload for Development](#compile-and-hot-reload-for-development)
    - [Lint with ESLint](#lint-with-eslint)
    - [Compile and Minify for Production](#compile-and-minify-for-production)
- [Deploy to gh-pages](#deploy-to-gh-pages)
- [Additional Docs](#additional-docs)

# Recommended IDE Setup

- IDE - [VSCode](https://code.visualstudio.com/)
- Extensions
  - [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur)
  - Markdown

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

# Project Setup

- Clone the repo
- Install nvm [node version manager](https://github.com/nvm-sh/nvm?tab=readme-ov-file#install--update-script)
- Install node with below commands

```sh
# install and uses node version from .nvmrc file
nvm use
# install packages from package.json
npm install
```

# Run localhost

### Sync checkout branch to latest chnages

```sh
 git fetch --all -p; git pull; git status;
 git merge origin/main
 git push;
```

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```

```sh
npm run format
```

### Compile and Minify for Production

```sh
npm run build
```

# Deploy to gh-pages

```sh
npm run deploy
```

# Additional Docs

- [Create New and Setup](./docs/README.md)
