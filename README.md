# notes

Something to keep in memory.

[中文](https://github.com/helvenk/notes/blob/master/README_zh.md)

## Node

### Develop with Typescript

Develop on node.js with `Typescript` using `babel-node` instead of `ts-node`(not working well).

Not meant for production use.

<details>
  <summary>Example</summary>
  <br/>

- add deps

```sh
yarn add @babel/node @babel/core @babel/preset-env @babel/preset-typescript nodemon -D
```

- add config in `package.json`

```js
"babel": {
  "presets": [
    "@babel/preset-env",
    "@babel/preset-typescript"
  ]
}
```

- use command

```sh
nodemon --exec babel-node ./src/index.ts --extensions .ts
```

</details>
