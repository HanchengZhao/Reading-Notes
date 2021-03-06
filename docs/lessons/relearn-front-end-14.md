# 浏览器-排版

1. 给`DOM`元素添加了用于展现的`css`属性后，浏览器下一步就是要确定每一个元素的位置。
2. 基本概念
   1. **排版**：确定浏览器元素的过程。
   2. **正常流排版**：浏览器的最基本排版方式，它包含了顺次排布和折行等规则，是唯一一个文字和盒排版的排版方式。
   3. **文字排版**：规定了行模型和文本在行模型中的排布，行模型规定了行顶，行底，文字区域、基线等对其方式。
   4. **盒模型**：浏览器中的元素被定义为占据长方形的区域，并允许边框，边距和留白。
   5. **绝对定位元素**：把自身从正常流种抽出，直接由 top 和 left 等属性确定自身的位置，不参加排版计算，也不影响其他元素，绝对定位 由 position 属性控制，需要根据它的包含块来确定位置，逐层找到其父级的 position 非 static 元素即可。
   6. **浮动元素**： 使得自己在正常流的位置向左或者向右移动到边界，并占据一块排版空间，该元素由 float 属性控制。
3. **主轴**： 文字依次书写的延伸方向，**交叉轴**：换行延伸的方向，跟主轴垂直交叉。
4. 文字排版除了字体提供的字形本身的信息，还收到一些`css`属性的影响：`line-height`、`letter-spacing`、`word-spacing`等。
5. `display`为`inline`的元素，是被拆成文本来排版的，而不是长方形盒。其主轴方向的`margin`和`border`也会被计算到排版中。
6. **浮动元素排版**：先排入正常流，再移动到排版宽度的最左/最右（主轴的最前和最后）。
7. **flex 排版**：将每一行排版后的剩余空间平均分配给主轴方向的`width`/`height`属性。
