# 项目说明

## honkit 项目结构

|   | |
| ------------- | ------------- |
| SUMMARY.md  | 项目目录  |
| README.md  | 项目主页  |

## 自定义插件 toggle-sidebar-url

官方没有提供默认隐藏sidebar功能，也没有找到类似插件，所以自己写了一个，

但由于插件功能会在正式功能之后加载，所以第一次打开会有页面闪动。

> 使用方法：在 链接后 加 `sidebar=false` 参数

## 自定义块处理插件：pre-html

使用方法：

md 文件中这样加
```
{% pre "font-size: 2em; font-weight: 700;", name="div" %}
test
{% endpre %}
```

会被编译成：
```
`<dev style='font-size: 2em; font-weight: 700;'>test</dev>`
```