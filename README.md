# 关于gitlab_README.md添加页面锚点的问题

####TOP
######【TOP为下文的测试做准备】

*  markdown添加页内锚点一般有两种方法

1.html标签实现
```
加入链接：<a href="jump">点击发生跳转</a>

定义一个锚（id）<span id="jump">要跳转的地方</span>
```

<a href="top">top</a>

<span id="top">跳转至顶部</span>

2.markdown语法实现

```
[name](#_)

<span id="">__</span>
```
[教务宝V1.1产品目录](#1)
<span id="1">产品目录</span>

上述两种方法在markdown编辑器中都可实现页面内部跳转
在gitlab中无法实现
最后发现gitlab无法识别中文+英文+数字的id
只要保证链的id是纯中文，纯英文即可

```
[教务宝V1.1目录](#目录_)
```
