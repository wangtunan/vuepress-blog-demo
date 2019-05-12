---
prev: false
next: /common/next1.md
---
# 基础配置功能

## 自动生成目录
[[toc]]

## 代码块高亮及行号
```js {2, 3, 4}
export default function sayHello () {
  console.log('Hello');
  console.log('World');
  console.log('!');
}
```

## 静态资源引用
```md
// 不使用别名引用
![不使用别名引用](~@vuepess/1.png)

// 使用别名引用
![使用别名引用](../images/vuepress/1.png)

```
### 不使用别名引用
![不使用别名引用](~@vuepress/1.png)

### 使用别名引用
![使用别名引用](../images/vuepress/1.png)

## 使用自定义样式
::: tip 提醒
你看到的红色代码块就是自定义样式的效果，它的路径在`.vuepress/style.styl`文件中
:::
`VuePress` 由两部分组成：一部分是支持用 `Vue` 开发主题的极简静态网站生成器，另一个部分是为书写技术文档而优化的默认主题。它的诞生初衷是为了支持 Vue 及其子项目的文档需求。<br/>

每一个由 `VuePress` 生成的页面都带有预渲染好的 `HTML`，也因此具有非常好的加载性能和搜索引擎优化（`SEO`）。同时，一旦页面被加载，`Vue` 将接管这些静态内容，并将其转换成一个完整的单页应用（`SPA`），其他的页面则会只在用户浏览到的时候才按需加载。

## 在Markdown中使用Vue组件
查看效果请点击此链接[在Markdown中使用Vue组件](/common/component.md)

## 引用已有的代码片段
<<< @/docs/.vuepress/js/hello.js {2}