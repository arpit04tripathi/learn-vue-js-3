# Setup

Below are the steps to setup and create new repo

- [Setup](#setup)
- [Initialize this repo](#initialize-this-repo)


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
