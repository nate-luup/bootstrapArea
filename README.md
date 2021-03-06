# bootstrapArea
This repo will be used for learn bootstrap

- [bootstrap.scss](#bootstrap-scss)
- [_functions.scss](_functions.scss.md)
- [_variables](_variables.scss.md)
- [_mixins](_mixins.scss.md)
- [_root.scss](_root.scss.md)
- [_reboot.scss](_reboot.scss.md)
- [Q&A](#question-answer)
- [参考地址](#reference)


<h2 id="bootstrap-scss">bootstrap.scss</h2>

```
// Configuration

@import "functions";
@import "variables"; //定义变量，方便后面调用
@import "mixins"; //定义混合 这类似定义函数或者宏，在mixins文件夹中可看到所定义的函数

@import "utilities";


// Layout & components

@import "root";
@import "reboot";
@import "type"; //排版样式
@import "images";
@import "grid"; //栅格系统，这是Bootstrap支持响应式的重点
@import "tables"; //表格样式
@import "forms"; //表单样式
@import "buttons"; //按钮样式
@import "transitions";
@import "dropdown"; //下拉菜单及下三角符号
@import "button-group"; //按钮组
@import "nav"; //导航
@import "navbar"; //导航条
@import "card";
@import "breadcrumb"; //面包屑
@import "pagination"; //默认分页
@import "badge"; //徽章
@import "alert"; //警告框
@import "progress"; //进度条
@import "list-group"; //列表组
@import "close"; //关闭按钮图标
@import "toasts";
@import "modal"; //模态框
@import "tooltip"; //工具提示
@import "popover"; //弹出框
@import "carousel"; //轮播
@import "spinners";


// Helpers

@import "helpers";


// Utilities

@import "utilities/api"; //实用工具类

```
<h2 id="question-answer">Q&A</h2>

- [TypeError on loading react-bootstrap](https://github.com/react-bootstrap/react-bootstrap/issues/4139)


<h2 id="reference">参考地址</h2>

- [Bootstrap中文手册](https://code.z01.com/v4/docs/)
- [目录结构](https://code.z01.com/v4/docs/contents.html)
- [Bootstrap源码分析系列之整体架构](https://www.cnblogs.com/jesse131/p/5966145.html)
- [Bootstrap源码分析系列之初始化和依赖项](https://www.cnblogs.com/jesse131/p/5974819.html)
- [Bootstrap源码分析系列之核心CSS](cnblogs.com/jesse131/p/5988125.html)
- [40 个超棒的免费 Bootstrap HTML5 网站模板](https://www.oschina.net/news/59924/free-bootstrap-templates)
