# test-nuxt

> My well-made Nuxt.js project

## Build Setup

``` bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
 
## Step
1. initialize project
```
npx create-nuxt-app test-nuxt
```
2. install these package for cross-platform files.
```
npm i -D copyfiles rimraf
```
3. Edit npm script

```diff
scripts: {
  ...
+ "build-docs": "rimraf docs && npm run generate && copyfiles --up 1 \"dist/**/*\" \"docs/\"",
  ...
}

```
4. Run build below.
