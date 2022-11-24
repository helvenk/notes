# 疑难杂症

### Mac M1 用 nvs 安装 node.js 失败

nvs 默认找 arm64 架构的 node.js 来安装，且该版本不支持 arm 架构，直接指定安装 x64 版本即可。
```sh
nvs add 14/x64
```
