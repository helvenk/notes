# notes

随便写写

[English](https://github.com/helvenk/notes/blob/master/README.md)

## Node

### 使用 Typescript 开发

使用 `Typescript` 开发 node.js 项目， 用 `babel-node` 实时编译运行， 不使用 `ts-node`(问题太多)。

仅在开发模式下使用，生产环境建议走 babel 打包。

<details>
  <summary>示例</summary>
  <br/>

- 安装依赖

```sh
yarn add @babel/node @babel/core @babel/preset-env @babel/preset-typescript nodemon -D
```

- 在 `package.json` 添加 babel 配置

```js
"babel": {
  "presets": [
    "@babel/preset-env",
    "@babel/preset-typescript"
  ]
}
```

- 使用下面的命令或者添加到 `scripts`

```sh
nodemon --exec babel-node ./src/index.ts --extensions .ts
```

</details>
