# get

[![GPL-3.0](https://img.shields.io/badge/license-GPL--3.0-blue.svg)](LICENSE)

https://www.mtdhb.com 红包核心领取逻辑，需配合 [mtdhb/api](https://github.com/mtdhb/api) 使用

基于 [mtdhb/old](https://github.com/mtdhb/old) 改造，代码比较乱，自行研究和部署吧

## 版本

master 分支为本站服务器正在跑的版本，可能含有临时调试代码

[查看稳定版本](https://github.com/mtdhb/get/releases)

## 环境

Node.js 9.x

## 代理

修改 [src/service/proxy-server.js](src/service/proxy-server.js) 代理服务器配置

如果只有一个代理，也可以只配置服务器环境变量

```bash
export PROXY_HOST=ip
export PROXY_PORT=port
```

## 开发

```bash
npm i
npm run dev
```

## 生产

* 首次部署

```bash
npm i pm2 -g
npm i
npm start
```

* 代码更新

```bash
npm run reload
```
