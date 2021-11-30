# vue-smart-campus

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

## 安装element-ui

```plain
npm install element-ui --save
```

src目录下的main.js，引入element-ui依赖

```plain
import Element from 'element-ui'
import "element-ui/lib/theme-chalk/index.css"
Vue.use(Element)
```

安装axios（[http://www.axios-js.com/](http://www.axios-js.com/?fileGuid=HXqVy6jx8qkWKPJq)），axios是一个基于 promise 的 HTTP 库，这样我们进行前后端对接的时候，使用这个工具可以提高我们的开发效率。

```plain
npm install axios --save
```

在main.js中全局引入axios。

```plain
import axios from 'axios'
Vue.prototype.$axios = axios //
```

qs是一个流行的查询参数序列化和解析库。可以将一个普通的object序列化成一个查询字符串，或者反过来将一个查询字符串解析成一个object,帮助我们查询字符串解析和序列化字符串。

```plain
npm install qs --save
```

然后因为后台我们现在还没有搭建，无法与前端完成数据交互，因此我们这里需要mock数据，因此我们引入mockjs（[http://mockjs.com/](http://mockjs.com/?fileGuid=HXqVy6jx8qkWKPJq)），方便后续我们提供api返回数据。

```plain
npm install mockjs --save-dev
```

```plain
require("./mock") //引入mock数据，关闭则注释该行
```







