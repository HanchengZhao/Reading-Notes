# `HTML`语义

1. 语义类标签的好处：
   1. 增强可读性，页面结构清晰，便于团队的开发和维护
   2. 有益于搜索引擎检索（`SEO`），支持读屏软件，根据文章自动生成目录等。
2. 对于语义标签，**用对**比**不用**好，**不用**比**用错**好。
3. 语义标签的**4**种使用场景：
   1. 自然语言能力的补充（注解）
   2. `HTML`有些标签是必须的，如果没有，文字会产生歧义。例如某种场景下表示强调的`em`
   3. 文章标题摘要，例如：`h1`-`h6`,`hgroup` 4.适合机器阅读的整体结构
4. 一个典型的`body`结构类似：

   ```htmlbars
   <body>
       <header>
           <nav>
               ……
           </nav>
       </header>
       <aside>
           <nav>
               ……
           </nav>
       </aside>
       <section>……</section>
       <section>……</section>
       <section>……</section>
       <footer>
           <address>……</address>
       </footer>
   </body>
   ```

5. 在上述结构里的标签说明：
   1. `header`通常出现在前部，表示导航或介绍性内容。
   2. `footer` 通常出现在尾部，包含一些作者信息、相关链接、版权信息等。通常它和`header`都是放在`article`或者`body`的直接子元素。
   3. `aside`表示跟文章主体不那么相关的部分，它可能包含导航、广告等工具性质的内容。侧边栏是`aside`，`aside`不一定是侧边栏。
   4. `aside` 和 `header` 中都可能出现导航（nav 标签），二者的区别是，`header` 中的导航多数是到文章自己的目录，而 `aside` 中的导航多数是到关联页面或者是整站地图。
   5. `footer`中的`address`表示作者信息。