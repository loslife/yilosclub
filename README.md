yilosclub
=========

基于Node Club的乐斯社区系统，感谢 Node Club！


## 介绍

Node Club 是用 **Node.js** 和 **MongoDB** 开发的新型社区软件

## 安装部署

```bash
// install node npm mongodb
// run mongod
$ npm install
$ cp config.default.js config.js
// modify the config file as yours
$ node app.js
```

## TEST

```bash
$ make test
```

jscoverage

```bash
$ make test-cov
```

* jscoverage: [**31%**](http://fengmk2.github.com/coverage/nodeclub.html)

## 其它

小量修改了两个依赖模块：node-markdown

* node-markdown/lib/markdown.js

allowedTags 添加：

```
embed  //支持 flash 视频
table|thead|tbody|tr|td|th|caption  //支持表格
```

allowedAttributes 添加：

```
embed:'src|quality|width|height|align|allowScriptAccess|allowFullScreen|mode|type'
table: 'class'