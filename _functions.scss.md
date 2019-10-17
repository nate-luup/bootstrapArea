
# Bootstrap functions

Utility mixins and functions for evaluating source code across our variables, maps, and mixins.
- @mixin
    - **Ascending** Ascending *Used to evaluate Sass maps like our grid* breakpoints.
    - **Starts at zero** Starts at zero *Used to ensure the min-width of the* lowest breakpoint starts at 0.
- @function
    - **negativify-map**  Turn maps into its negative variant
    - **map-get-multiple** Get multiple keys from a sass map
    - **str-replace**
    - **escape-svg**  See https://codepen.io/kevinweber/pen/dXWoRw
    - **color-yiq** Color contrast
    - **color-level** Request a color level
- [Reference](#reference)
<h2 id="reference">Reference</h2>

- [SASS用法指南](http://ruanyifeng.com/blog/2012/06/sass.html)
- [Sass内建函数用法一览](http://jimyuan.github.io/blog/2017/06/07/sass-preset-functions-learning.html)
- [mixins](http://sass.bootcss.com/docs/sass-reference/#mixins)
- [unit()函数](https://www.imooc.com/code/8450)
> unit() 函数主要是用来获取一个值所使用的单位，碰到复杂的计算时，其能根据运算得到一个“多单位组合”的值，不过只充许乘、除运算
```
>> unit(100)
""
>> unit(100px)
"px"
>> unit(20%)
"%"
>> unit(1em)
"em"
>> unit(10px * 3em)
"em*px"
>> unit(10px / 3em)
"px/em"
>> unit(10px * 2em / 3cm / 1rem)
"em/rem"
```
- [comparable($number1, $number2)] 
> 返回一个布尔值，判断传入的两个数值是否是可以进行比较或计算的。
- [@each](https://sass-lang.com/documentation/at-rules/control/each)



