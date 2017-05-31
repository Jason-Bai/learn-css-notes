一、概述

> font 简写属性在一个声明中设置所有字体属性。

注释：此属性也有


二、说明

这个简写属性用于一次设置元素字体的两个或更多方面。使用 icon 等关键字可以适当地设置元素的字体，使之与用户计算机环境中的某个方面一致。注意，如果没有使用这些关键词，至少要指定字体大小和字体系列。

可以按顺序设置如下属性：

* font-style
* font-variant
* font-weight
* font-size/line-height
* font-family

可以不设置其中的某个值，比如 font:100% verdana; 也是允许的。未设置的属性会使用其默认值。

三、可能的值

| 值 | 描述 |
| ---- | ---- |
| _font-style_ | 规定字体样式。参阅：[font-style](/cssref/pr_font_font-style.asp "CSS font-style 属性") 中可能的值。 |
| _font-variant_ | 规定字体异体。参阅：[font-variant](/cssref/pr_font_font-variant.asp "CSS font-variant 属性") 中可能的值。 |
| _font-weight_ | 规定字体粗细。参阅：[font-weight](/cssref/pr_font_weight.asp "CSS font-weight 属性") 中可能的值。 |
| _font-size/line-height_ | 规定字体尺寸和行高。参阅：[font-size](/cssref/pr_font_font-size.asp "CSS font-size 属性") 和 [line-height](/cssref/pr_dim_line-height.asp "CSS line-height 属性") 中可能的值。 |
| _font-family_ | 规定字体系列。参阅：[font-family](/cssref/pr_font_font-family.asp "CSS font-family 属性") 中可能的值。 |
| caption | 定义被标题控件（比如按钮、下拉列表等）使用的字体。 |
| icon | 定义被图标标记使用的字体。 |
| menu | 定义被下拉列表使用的字体。 |
| message-box | 定义被对话框使用的字体。 |
| small-caption | caption 字体的小型版本。 |
| status-bar | 定义被窗口状态栏使用的字体。 |
