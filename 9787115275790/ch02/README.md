|本期版本| 上期版本
|:---:|:---:
`Wed Jan 12 22:59:05 CST 2022` | -

# 第 2 章 在HTML 中使用 JavaScript 


**服务器端脚本语言动态生成 JavaScript**

```
include ActionController::MimeResponds
respond_to :js

index.js.erb
```

### 2.1.1 标签的位置

* 现代 web 应用程序一般都把全部 JavaScript 引用放在 body 的元素中页面内容的后面

### 2.1.4 在XHTML中的用法

```
<script type="text/javascript">
//<![CDATA[

//]]>
</script>
```

## 2.3 文档模式

* 混杂 模式（quirks mode）和标准模式（standards mode）
* 虽然这两种模式的主要区别只体现在通过 CSS 渲染的内容方面，但对 JavaScript 也有一些关联影响，或称为副作用
* 准标准模式（almost standards mode）

## Ref

* [看了你就懂的同步与异步、阻塞与非阻塞](https://segmentfault.com/a/1190000022478666)
* [MIME 类型](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Basics_of_HTTP/MIME_types) / [常见 MIME 类型列表](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Common_types)
* [怪异模式和标准模式](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Quirks_Mode_and_Standards_Mode#how_does_mozilla_determine_which_mode_to_use.3f)
