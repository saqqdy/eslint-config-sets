# eslint-config-sets

eslint 规则预设

[![NPM version][npm-image]][npm-url]
[![Codacy Badge][codacy-image]][codacy-url]
[![Known Vulnerabilities][snyk-image]][snyk-url]
[![npm download][download-image]][download-url]
[![License][license-image]][license-url]

[![Sonar][sonar-image]][sonar-url]

[npm-image]: https://img.shields.io/npm/v/eslint-config-sets.svg?style=flat-square
[npm-url]: https://npmjs.org/package/eslint-config-sets
[codacy-image]: https://app.codacy.com/project/badge/Grade/f70d4880e4ad4f40aa970eb9ee9d0696
[codacy-url]: https://www.codacy.com/gh/saqqdy/eslint-config-sets/dashboard?utm_source=github.com&utm_medium=referral&utm_content=saqqdy/eslint-config-sets&utm_campaign=Badge_Grade
[snyk-image]: https://snyk.io/test/npm/eslint-config-sets/badge.svg?style=flat-square
[snyk-url]: https://snyk.io/test/npm/eslint-config-sets
[download-image]: https://img.shields.io/npm/dm/eslint-config-sets.svg?style=flat-square
[download-url]: https://npmjs.org/package/eslint-config-sets
[license-image]: https://img.shields.io/badge/License-MIT-blue.svg
[license-url]: LICENSE
[sonar-image]: https://sonarcloud.io/api/project_badges/quality_gate?project=saqqdy_eslint-config-sets
[sonar-url]: https://sonarcloud.io/dashboard?id=saqqdy_eslint-config-sets

## 安装依赖

### vue 安装插件

```shell
npm install -D eslint-plugin-vue eslint-plugin-vue-scoped-css eslint-plugin-jsdoc babel-eslint eslint prettier vue-eslint-parser
```

### vue3.0 安装插件

```shell
npm install -D eslint-plugin-vue eslint-plugin-vue-scoped-css @vue/eslint-config-prettier eslint-plugin-jsdoc babel-eslint eslint prettier vue-eslint-parser
```

### vue3.0 typescript 版本安装插件

```shell
npm install -D eslint-plugin-vue eslint-plugin-vue-scoped-css @vue/eslint-config-prettier eslint-plugin-tsdoc babel-eslint eslint prettier vue-eslint-parser @typescript-eslint/eslint-plugin @typescript-eslint/parser @vue/cli-plugin-typescript @vue/eslint-config-typescript typescript
```

### vue3.0 typescript library 版本安装插件

```shell
npm install -D eslint-plugin-vue eslint-plugin-tsdoc eslint-plugin-import eslint-plugin-prettier eslint-config-prettier babel-eslint eslint prettier vue-eslint-parser @typescript-eslint/eslint-plugin @typescript-eslint/parser typescript
```

### react 安装插件

```shell
npm install -D eslint-plugin-jsdoc babel-eslint eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-import eslint prettier
```

### react typescript 安装插件

```shell
npm install -D eslint-plugin-tsdoc babel-eslint eslint-plugin-react eslint-plugin-react-hooks eslint-plugin-import eslint prettier @typescript-eslint/eslint-plugin @typescript-eslint/parser typescript
```

### egg 安装插件

```shell
npm install -D eslint-config-egg eslint prettier babel-eslint
```

### simple 安装插件

```shell
npm install -D eslint prettier babel-eslint
```

### simple typescript 安装插件

```shell
npm install -D eslint prettier babel-eslint eslint-plugin-tsdoc @typescript-eslint/eslint-plugin @typescript-eslint/parser typescript
```

### nuxt 安装插件

```shell
npm install -D eslint prettier babel-eslint @nuxtjs/eslint-config @nuxtjs/eslint-module eslint-config-prettier eslint-plugin-jsdoc eslint-plugin-nuxt eslint-plugin-prettier@8.x vue-eslint-parser
```

## 使用

### 配置说明

eslint-config-sets 包含了下面这几套配置

-   `egg`: eggjs 项目
-   `nuxt`: 基于 nuxt 的项目
-   `react`: create-react-app 创建的项目
-   `reactTs`: create-react-app 创建的 typescript 项目
-   `vue`: vue 全家桶项目
-   `vue3`: vue3.0 项目
-   `vue3Ts`: vue3.0 typescript 项目
-   `simple`: node lib 项目
-   `simpleTs`: node lib typescript 项目

### 引入方法

1. 在 `vue3.0` 项目中使用

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

2. 在 `vue3.0 typescript` 项目中使用

    ```js
    // .eslintrc.js
    const { vue3Ts: config } = require('eslint-config-sets')
    // ...同上
    ```

3. 在 `vue3.0 typescript library` 项目中使用

    ```js
    // .eslintrc.js
    const { vue3TsLib: config } = require('eslint-config-sets')
    // ...同上
    ```

4. 在 `react` 项目中使用

    ```js
    // .eslintrc.js
    const { react: config } = require('eslint-config-sets')
    // ...同上
    ```

5. 在 `react typescript` 项目中使用

    ```js
    // .eslintrc.js
    const { reactTs: config } = require('eslint-config-sets')
    // ...同上
    ```

6. 在 `egg` 项目中使用

    ```js
    // .eslintrc.js
    const { egg: config } = require('eslint-config-sets')
    // ...同上
    ```

7. 在 `nuxt` 项目中使用

    ```js
    // .eslintrc.js
    const { nuxt: config } = require('eslint-config-sets')
    // ...同上
    ```

8. 在 `js lib` 项目中使用

    ```js
    // .eslintrc.js
    const { simple: config } = require('eslint-config-sets')
    // ...同上
    ```
