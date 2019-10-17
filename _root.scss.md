# 目录结构
- [变量声明](_variables.scss.md)
- [源代码](#source-code)
- [代码解析](#code-analysis)
- [生成代码](#result)
- [参考地址](#reference)

<h2 id="source-code">源代码</h2>

```
:root {
  // Custom variable values only support SassScript inside `#{}`.
  @each $color, $value in $colors {
    --#{$color}: #{$value};
  }

  @each $color, $value in $theme-colors {
    --#{$color}: #{$value};
  }

  // Use `inspect` for lists so that quoted items keep the quotes.
  // See https://github.com/sass/sass/issues/2383#issuecomment-336349172
  --font-family-sans-serif: #{inspect($font-family-sans-serif)};
  --font-family-monospace: #{inspect($font-family-monospace)};
}
```
<h2 id="code-analysis">代码解析</h2>

**作用：** 生成css全局变量

**包含内容：** 
- 基础颜色
- 主题颜色
- 字体定义

<h2 id="result">生成代码</h2>

```
:root {
  --blue: #0d6efd;
  --indigo: #6610f2;
  --purple: #6f42c1;
  --pink: #d63384;
  --red: #dc3545;
  --orange: #fd7e14;
  --yellow: #ffc107;
  --green: #28a745;
  --teal: #20c997;
  --cyan: #17a2b8;
  --white: #fff;
  --gray: #6c757d;
  --gray-dark: #343a40;
  --primary: #0d6efd;
  --secondary: #6c757d;
  --success: #28a745;
  --info: #17a2b8;
  --warning: #ffc107;
  --danger: #dc3545;
  --light: #f8f9fa;
  --dark: #343a40;
  --font-family-sans-serif: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
  --font-family-monospace: SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
}
```

<h2 id="reference">参考地址</h2>

- [css变量](https://developer.mozilla.org/zh-CN/docs/Web/CSS/Using_CSS_custom_properties)
- [Scss @each](https://sass-lang.com/documentation/at-rules/control/each)
- [Sass Maps](https://aotu.io/notes/2015/12/09/an-introduction-to-sass-maps/index.html)