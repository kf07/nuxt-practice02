# nuxt-practice02

> My prime Nuxt.js project

## Build Setup

``` bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm start
　
# generate static project
$ npm run generate
```

For detailed explanation on how things work, checkout [Nuxt.js docs](https://nuxtjs.org).

##layout
特に指定しない場合/layout/default.vueが使用される

別のレイアウトを指定する場合は/layout/***.vueで作成して
ページコンポーネントのlayoutキーに指定

```javascript
export default {
  layout: 'single'
}
```
default.vueをトップページ用、下層ページをsingle.vue等とした場合、下層ページ全てに layout: 'single'を指定しなければいけないため、default.vueを下層ページ用にして、home.vue等をトップページ用のレイアウトにするのが良い
