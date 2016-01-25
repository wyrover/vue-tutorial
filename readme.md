# vue-tutorial

vue 可以在前端页面直接引用，也可以用 webpack 直接打包，对于大型工程来说用 webpack 打包比较合适，也适合写组件。


vue 官方提供了 vue-cli 来生成应用程序骨架。这个命令行有四种使用方式

|     |     |
| ----- | ----- |
|browserify |A full-featured Browserify + vueify setup with hot-reload, linting & unit testing.|
|browserify-simple |A simple Browserify + vueify setup for quick prototyping.|
|webpack |A full-featured Webpack + vue-loader setup with hot reload, linting, testing & css extraction.|
|webpack-simple |A simple Webpack + vue-loader setup for quick prototyping.|

另外两种

-  vue init username/repo my-project
-  vue init ~/fs/path/to-custom-template my-project

```
npm install -g vue-cli
```


例子

```
vue init webpack my-project
cd my-project
npm install
npm run dev
```
[http://localhost:8080](http://localhost:8080)


|     |     |
| ----- | ----- |
|[vue-loader 文档](https://vuejs.github.io/vue-loader/) | |
|[sublime 的 vue 语法高亮插件](https://github.com/vuejs/vue-syntax-highlight) | |
|[vue-hackernews](https://github.com/vuejs/vue-hackernews) | |
|[vue-base](https://github.com/szarapka/vue-base) | |
|[GB-webpack](https://github.com/viko16/GB-webpack) | |
|[vue-vueRouter-webpack-example](https://github.com/hilongjw/vue-vueRouter-webpack-example) | |
|[vue-desktop-starter](https://github.com/ElemeFE/vue-desktop-starter) | |
|[vue-desktop](https://github.com/ElemeFE/vue-desktop)     | |
|[V2EX-mobile](https://github.com/Vincent1993/V2EX-mobile) | |
|[blog-webui-vue](https://github.com/iAmHades/blog-webui-vue) | |
|[electron-boilerplate-vue](https://github.com/bradstewart/electron-boilerplate-vue) |electron 和 vue.js 结合 |
|[vue-electron](https://github.com/rodzzlessa24/vue-electron) | |
|[vue-electron-bp](https://github.com/tuommii/vue-electron-bp) | |
|[Atom-Electron-Vue.js](https://github.com/phleobon/Atom-Electron-Vue.js) | |
|[rss-reader](https://github.com/mrgodhani/rss-reader) | |
|[vue-webgulp](https://github.com/rodzzlessa24/vue-webgulp) |使用 gulp + webpack 结合的工程|
|[vue-skeleton](https://github.com/rodzzlessa24/vue-skeleton) | |
|[goldminers](https://github.com/zhangweijie-cn/goldminers) |基于 Electron 和 Vue.js 打造的掘金贡献者排行榜 |
|[idaxiang](https://github.com/zhangweijie-cn/idaxiang) |大象公会桌面客户端|
|[JSONformatter](https://github.com/ablipan/JSONformatter) | |
|[themekit-vue](https://github.com/themekit/themekit-vue) | |
|[vue-markdown-editor](https://github.com/themekit/vue-markdown-editor) | |
|[v-datepicker](https://github.com/ElemeFE/v-datepicker)   |日期组件|
|[vue-infinite-scroll](https://github.com/ElemeFE/vue-infinite-scroll) |无限滚动|
|[vue-swipe](https://github.com/ElemeFE/vue-swipe) | |
|[vue-jwt](https://github.com/rodzzlessa24/vue-jwt) | |
|[vue-jwt-authentication](https://github.com/auth0/vue-jwt-authentication) |Vue.js JWT Authentication |
|[vue-validator](https://github.com/vuejs/vue-validator) | |
|[vue-calendar](https://github.com/jinzhe/vue-calendar) | |
|[vue-lazyload](https://github.com/hilongjw/vue-lazyload) | |
|[vueify-example](https://github.com/vuejs/vueify-example) | |
|[Laravel-Elixir-Vueify-Setup](https://github.com/laracasts/Laravel-Elixir-Vueify-Setup) | |
|[vue-ghpages-blog](https://github.com/viko16/vue-ghpages-blog) | |
|[webpack-demos](https://github.com/ruanyf/webpack-demos) | |
|[lumenvue](https://github.com/bestmomo/lumenvue) |A simple tutorial application of Lumen and vue.js |
|[vuejs-book](https://github.com/koba04/vuejs-book) | |
|[vue-material-blog](https://github.com/hilongjw/vue-material-blog) | |

## 使用 SASS 的组件模板
```
<template>
  <div class="example">{{ msg }}</div>
</template>

<script>
export default {
  data () {
    return {
      msg: 'Hello world!'
    }
  }
}
</script>

<style lang="sass">

</style>
```

## 配置 Hot Reload

```
// package.json
...
"scripts": {
  "dev": "webpack-dev-server --inline --hot"
}
...
```