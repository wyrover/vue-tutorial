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
|[vue-loader 文档](https://vuejs.github.io/vue-loader/)| |
|[sublime 的 vue 语法高亮插件](https://github.com/vuejs/vue-syntax-highlight)| |
|[vue-hackernews](https://github.com/vuejs/vue-hackernews)| |
|[vue-base](https://github.com/szarapka/vue-base)| |
|[vue-desktop-starter](https://github.com/ElemeFE/vue-desktop-starter)| |
|[vue-desktop](https://github.com/ElemeFE/vue-desktop)     | |
|[v-datepicker](https://github.com/ElemeFE/v-datepicker)   |日期组件|


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