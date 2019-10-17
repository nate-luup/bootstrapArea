# bootstrapArea
This repo will be used for learn bootstrap

- [scss目录结构](#dir)
- [bootstrap.scss](#bootstrap-scss)
- [_functions.scss](_functions.scss.md)
- [_variables](_variables.scss.md)
- [_mixins](_mixins.scss.md)
- [_root.scss](_root.scss.md)
- [_reboot.scss](_reboot.scss.md)
- [Q&A](#question-answer)
- [参考地址](#reference)

<h2 id="dir">scss目录结构</h2>

 ```   
scss/
├── _alert.scss 
├── _badge.scss
├── _breadcrumb.scss
├── _button-group.scss
├── _buttons.scss
├── _card.scss
├── _carousel.scss
├── _close.scss
├── _dropdown.scss
├── _forms.scss
├── _functions.scss
├── _grid.scss
├── _helpers.scss
├── _images.scss
├── _list-group.scss
├── _mixins.scss
├── _modal.scss
├── _nav.scss
├── _navbar.scss
├── _pagination.scss
├── _popover.scss
├── _progress.scss
├── _reboot.scss
├── _root.scss
├── _spinners.scss
├── _tables.scss
├── _toasts.scss
├── _tooltip.scss
├── _transitions.scss
├── _type.scss
├── _utilities.scss
├── _variables.scss
├── bootstrap-grid.scss
├── bootstrap-reboot.scss
├── bootstrap-utilities.scss
├── bootstrap.scss
├── forms
│   ├── _form-check.scss
│   ├── _form-control.scss
│   ├── _form-file.scss
│   ├── _form-range.scss
│   ├── _form-select.scss
│   ├── _input-group.scss
│   ├── _labels.scss
│   ├── _layout.scss
│   └── _validation.scss
├── helpers
│   ├── _background.scss
│   ├── _clearfix.scss
│   ├── _colored-links.scss
│   ├── _embed.scss
│   ├── _position.scss
│   ├── _screenreaders.scss
│   ├── _stretched-link.scss
│   └── _text-truncation.scss
├── mixins
│   ├── _alert.scss
│   ├── _background-variant.scss
│   ├── _border-radius.scss
│   ├── _box-shadow.scss
│   ├── _breakpoints.scss
│   ├── _buttons.scss
│   ├── _caret.scss
│   ├── _clearfix.scss
│   ├── _deprecate.scss
│   ├── _forms.scss
│   ├── _gradients.scss
│   ├── _grid-framework.scss
│   ├── _grid.scss
│   ├── _image.scss
│   ├── _list-group.scss
│   ├── _lists.scss
│   ├── _pagination.scss
│   ├── _reset-text.scss
│   ├── _resize.scss
│   ├── _screen-reader.scss
│   ├── _table-row.scss
│   ├── _text-truncate.scss
│   ├── _transition.scss
│   └── _utilities.scss
├── utilities
│   └── _api.scss
└── vendor
    └── _rfs.scss
 ```   

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

1. [Flex-grow in IE11 doesn't vertically stretch](https://stackoverflow.com/questions/39609883/flex-grow-in-ie11-doesnt-vertically-stretch)


<h2 id="reference">参考地址</h2>

- [Bootstrap源码分析系列之整体架构](https://www.cnblogs.com/jesse131/p/5966145.html)
- [Bootstrap源码分析系列之初始化和依赖项](https://www.cnblogs.com/jesse131/p/5974819.html)
- [Bootstrap源码分析系列之核心CSS](cnblogs.com/jesse131/p/5988125.html)
- [sass-documentation](https://sass-lang.com/documentation)