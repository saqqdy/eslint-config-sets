# eslint 规则

[![NPM version][npm-image]][npm-url]
[![build status][travis-image]][travis-url]
[![Test coverage][codecov-image]][codecov-url]
[![David deps][david-image]][david-url]
[![Known Vulnerabilities][snyk-image]][snyk-url]
[![npm download][download-image]][download-url]

[npm-image]: https://img.shields.io/npm/v/eslint-config-sets.svg?style=flat-square
[npm-url]: https://npmjs.org/package/eslint-config-sets
[travis-image]: https://travis-ci.org/saqqdy/eslint-config-sets.svg?branch=master
[travis-url]: https://travis-ci.org/saqqdy/eslint-config-sets
[codecov-image]: https://img.shields.io/codecov/c/github/saqqdy/eslint-config-sets.svg?style=flat-square
[codecov-url]: https://codecov.io/github/saqqdy/eslint-config-sets?branch=master
[david-image]: https://img.shields.io/david/saqqdy/eslint-config-sets.svg?style=flat-square
[david-url]: https://david-dm.org/saqqdy/eslint-config-sets
[snyk-image]: https://snyk.io/test/npm/eslint-config-sets/badge.svg?style=flat-square
[snyk-url]: https://snyk.io/test/npm/eslint-config-sets
[download-image]: https://img.shields.io/npm/dm/eslint-config-sets.svg?style=flat-square
[download-url]: https://npmjs.org/package/eslint-config-sets

# 安装依赖

## vue 安装插件

```shell
npm install -D eslint-plugin-vue eslint-plugin-vue-scoped-css eslint-plugin-jsdoc babel-eslint eslint prettier vue-eslint-parser
```

## vue3.0 安装插件

```shell
npm install -D eslint-plugin-vue @vue/eslint-config-prettier eslint-plugin-jsdoc babel-eslint eslint prettier vue-eslint-parser
```

## vue3.0 typescript 版本安装插件

```shell
npm install -D eslint-plugin-vue @vue/eslint-config-prettier eslint-plugin-jsdoc babel-eslint eslint prettier vue-eslint-parser @typescript-eslint/eslint-plugin @typescript-eslint/parser @vue/cli-plugin-typescript @vue/eslint-config-typescript typescript
```

## react 安装插件

```shell
npm install -D @vue/eslint-config-prettier eslint-plugin-jsdoc babel-eslint eslint-plugin-react eslint-plugin-import eslint prettier
```

## react-ts 安装插件

```shell
npm install -D @vue/eslint-config-prettier eslint-plugin-jsdoc babel-eslint eslint-plugin-react eslint-plugin-import eslint prettier @typescript-eslint/eslint-plugin @typescript-eslint/parser typescript
```

## egg 安装插件

```shell
npm install -D eslint-config-egg eslint prettier babel-eslint
```

## simple 安装插件

```shell
npm install -D eslint prettier babel-eslint
```

## nuxt 安装插件

```shell
npm install -D eslint prettier babel-eslint @nuxtjs/eslint-config @nuxtjs/eslint-module eslint-config-prettier eslint-plugin-jsdoc eslint-plugin-nuxt eslint-plugin-prettier@8.x vue-eslint-parser
```

# 使用

## 配置说明

eslint-config-sets 包含了下面这几套配置

-   `egg`: eggjs 项目
-   `nuxt`: 基于 nuxt 的项目
-   `react`: create-react-app 创建的项目
-   `reactTs`: create-react-app 创建的 typescript 项目
-   `vue`: vue 全家桶项目
-   `vue3`: vue3.0 项目
-   `vue3Ts`: vue3.0 typescript 项目
-   `simple`: node lib 项目

## 引入方法

1. 在 vue3.0 项目中使用

```js
// .eslintrc.js
const { vue3: config } = require('eslint-config-sets')
module.exports = Object.assign(config, {
    rules: {
        // 自定义规则
        // semi: [2, 'never']
    }
})
```

2. 在 vue3.0 typescript 项目中使用

```js
// .eslintrc.js
const { vue3Ts: config } = require('eslint-config-sets')
// ...同上
```

3. 在 react 项目中使用

```js
// .eslintrc.js
const { react: config } = require('eslint-config-sets')
// ...同上
```

4. 在 egg 项目中使用

```js
// .eslintrc.js
const { egg: config } = require('eslint-config-sets')
// ...同上
```
