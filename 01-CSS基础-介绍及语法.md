一、 CSS概述：
> CSS是指层叠样式表，早期的时候页面中的样式是和html写在一起的，开始的时候没什么问题，但是随着页面内容的丰富及复杂后，大家发现写在一起太麻烦了，后来就把样式的部分抽离出来，这样就极大地提高了我们的工作效率。比喻的形象一下，html就好像我们的骨骼，CSS就是我们如果进行打扮自己，比如蓝色牛仔裤，白色特恤衫，拉风的帽子等。

二、选择器

| 选择器 | 例子 | 例子描述 | CSS |
| ---- | ---- | ---- | ---- |
| .class | .intro | 选择 class="intro" 的所有元素。| 1 |
| #id | #firstname | 选择 id="firstname" 的所有元素。 | 1 |
| * | * | 选择所有元素。 | 2|
| element | p | 选择所有<p>元素 | 1|
| element,element | div,p | 选择所有 <div> 元素和所有 <p> 元素。| 1 |
| element element | div p | 选择 <div> 元素内部的所有 <p> 元素。 | 1 |
| element > element | div > p | 选择父元素为 <div> 元素的所有 <p> 元素。| 2 |
| element+element | div+p | 选择紧接在 <div> 元素之后的所有 <p> 元素。| 2 |
| [attribute] | [target] | 选择带有 target 属性所有元素。 | 2 |
| [attribute=value] | [target=_blank] | 选择 target="_blank" 的所有元素。 | 2 |
| [attribute~=value] | [title~=flower] | 选择 title 属性包含单词 "flower" 的所有元素。 | 2 |
| [attribute!=value] | [title!=flower] | 选择 lang 属性值以 "en" 开头的所有元素。| 2 |
| :link | a:link | 选择所有未被访问的链接。| 1 |
| :visited | a:visited | 选择所有已被访问的链接。| 1 |
| :active | a:active | 选择活动链接。| 1 |
| :hover | a:hover | 选择鼠标指针位于其上的链接。| 1 |
| :focus | a:focus | 选择获得焦点的 input 元素。| 2 |
| [:first-letter](/cssref/selector_first-letter.asp "CSS :first-letter 选择器") | p:first-letter | 选择每个 <p> 元素的首字母。 | 1 |
| [:first-line](/cssref/selector_first-line.asp "CSS :first-line 选择器") | p:first-line | 选择每个 <p> 元素的首行。 | 1 |
| [:first-child](/cssref/selector_first-child.asp "CSS :first-child 选择器") | p:first-child | 选择属于父元素的第一个子元素的每个 <p> 元素。 | 2 |
| [:before](/cssref/selector_before.asp "CSS :before 选择器") | p:before | 在每个 <p> 元素的内容之前插入内容。 | 2 |
| [:after](/cssref/selector_after.asp "CSS :after 选择器") | p:after | 在每个 <p> 元素的内容之后插入内容。 | 2 |
| [:lang(_language_)](/cssref/selector_lang.asp "CSS :lang(language) 选择器") | p:lang(it) | 选择带有以 "it" 开头的 lang 属性值的每个 <p> 元素。 | 2 |
| [_element1_~_element2_](/cssref/selector_gen_sibling.asp "CSS element1~element2 选择器") | p~ul | 选择前面有 <p> 元素的每个 <ul> 元素。 | 3 |
| [[_attribute_^=_value_]](/cssref/selector_attr_begin.asp "CSS [attribute^=value] 选择器") | a[src^="https"] | 选择其 src 属性值以 "https" 开头的每个 <a> 元素。 | 3 |
| [[_attribute_$=_value_]](/cssref/selector_attr_end.asp "CSS [attribute$=value] 选择器") | a[src$=".pdf"] | 选择其 src 属性以 ".pdf" 结尾的所有 <a> 元素。 | 3 |
| [[_attribute_*=_value_]](/cssref/selector_attr_contain.asp "CSS [attribute*=value] 选择器") | a[src*="abc"] | 选择其 src 属性中包含 "abc" 子串的每个 <a> 元素。 | 3 |
| [:first-of-type](/cssref/selector_first-of-type.asp "CSS :first-of-type 选择器") | p:first-of-type | 选择属于其父元素的首个 <p> 元素的每个 <p> 元素。 | 3 |
| [:last-of-type](/cssref/selector_last-of-type.asp "CSS :last-of-type 选择器") | p:last-of-type | 选择属于其父元素的最后 <p> 元素的每个 <p> 元素。 | 3 |
| [:only-of-type](/cssref/selector_only-of-type.asp "CSS :only-of-type 选择器") | p:only-of-type | 选择属于其父元素唯一的 <p> 元素的每个 <p> 元素。 | 3 |
| [:only-child](/cssref/selector_only-child.asp "CSS :only-child 选择器") | p:only-child | 选择属于其父元素的唯一子元素的每个 <p> 元素。 | 3 |
| [:nth-child(_n_)](/cssref/selector_nth-child.asp "CSS :nth-child(n) 选择器") | p:nth-child(2) | 选择属于其父元素的第二个子元素的每个 <p> 元素。 | 3 |
| [:nth-last-child(_n_)](/cssref/selector_nth-last-child.asp "CSS :nth-last-child(n) 选择器") | p:nth-last-child(2) | 同上，从最后一个子元素开始计数。 | 3 |
| [:nth-of-type(_n_)](/cssref/selector_nth-of-type.asp "CSS :nth-of-type(n) 选择器") | p:nth-of-type(2) | 选择属于其父元素第二个 <p> 元素的每个 <p> 元素。 | 3 |
| [:nth-last-of-type(_n_)](/cssref/selector_nth-last-of-type.asp "CSS :nth-last-of-type(n) 选择器") | p:nth-last-of-type(2) | 同上，但是从最后一个子元素开始计数。 | 3 |
| [:last-child](/cssref/selector_last-child.asp "CSS :last-child 选择器") | p:last-child | 选择属于其父元素最后一个子元素每个 <p> 元素。 | 3 |
| [:root](/cssref/selector_root.asp "CSS :root 选择器") | :root | 选择文档的根元素。 | 3 |
| [:empty](/cssref/selector_empty.asp "CSS :empty 选择器") | p:empty | 选择没有子元素的每个 <p> 元素（包括文本节点）。 | 3 |
| [:target](/cssref/selector_target.asp "CSS :target 选择器") | #news:target | 选择当前活动的 #news 元素。 | 3 |
| [:enabled](/cssref/selector_enabled.asp "CSS :enabled 选择器") | input:enabled | 选择每个启用的 <input> 元素。 | 3 |
| [:disabled](/cssref/selector_disabled.asp "CSS :disabled 选择器") | input:disabled | 选择每个禁用的 <input> 元素 | 3 |
| [:checked](/cssref/selector_checked.asp "CSS :checked 选择器") | input:checked | 选择每个被选中的 <input> 元素。 | 3 |
| [:not(_selector_)](/cssref/selector_not.asp "CSS :not(selector) 选择器") | :not(p) | 选择非 <p> 元素的每个元素。 | 3 |
| [::selection](/cssref/selector_selection.asp "CSS ::selection 选择器") | ::selection | 选择被用户选取的元素部分。 | 3 |

* 注意：信息来源[CSS Selector][]


[CSS Selector]: http://www.w3school.com.cn/cssref/css_selectors.asp "CSS Selector"
