# Nuxt.js 2.9 (SSR) + Firebase (hosting and cloud functions) Example

## Build & Deploy

``` bash
# Install dependencies
$ cd /path/to/<project-name>/functions && yarn install
$ cd /path/to/<project-name>/src && yarn install

# Build Nuxt app
$ npm run build

# Copy files for hosting
$ rm -rf public/*
$ cp -R functions/nuxt/dist/ public/assets
$ cp -R src/static/* public

# Deploy
$ firebase deploy
```

