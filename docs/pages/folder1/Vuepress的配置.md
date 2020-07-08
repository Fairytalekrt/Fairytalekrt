# Vuepress 的配置
位于docs/.vuepress/config.js

### base
*   类型: `string`
*   默认值: `/`

部署站点的基础路径，如果你想让你的网站部署到一个子路径下，你将需要设置它。如 GitHub pages，如果你想将你的网站部署到 `https://foo.github.io/bar/`，那么 `base` 应该被设置成 `"/bar/"`，它的值应当总是以斜杠开始，并以斜杠结束。

`base` 将会作为前缀自动地插入到所有以 `/` 开始的其他选项的链接中，所以你只需要指定一次。
### title
*   类型: `string`
*   默认值: `undefined`
网站的标题，它将会被用作所有页面标题的前缀，同时，默认主题下，它将显示在导航栏（navbar）上。

### head

*   类型: `Array`
*   默认值: `[]`
额外的需要被注入到当前页面的 HTML `<head>` 中的标签，每个标签都可以以 `[tagName, { attrName: attrValue }, innerHTML?]` 的格式指定，举个例子，增加一个自定义的 favicon：

```javascript
module.exports = {
    head: [
        ['link', {
            rel: 'icon',
            href: '/logo.png'
        }]
    ]
}
```

### port
*   类型: `number`
*   默认值: `8080`

指定 dev server 的端口。


### dest

*   类型: `string`
*   默认值: `.vuepress/dist`

指定 `vuepress build` 的输出目录。如果传入的是相对路径，则会基于 `process.cwd()` 进行解析。

具体更多查阅[https://vuepress.vuejs.org/zh/config/](https://vuepress.vuejs.org/zh/config/)
