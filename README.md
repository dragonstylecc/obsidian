# obsidian中文帮助手册
obsidian中文帮助手册由社群成员Leon，Linpean，Jackiexiao，蚕子等共同翻译。

本文内容由社区成员贡献。

### 如何使用帮助文档？
点击clone下载后或[这里](https://github.com/Jackiexiao/obsidian/archive/master.zip)，用obsidian打开（在设置按钮的上方`Open another vault`）即可。

* 中文交流Q群774176839，群文件中有obsidian汉化包
* [官网、下载地址](https://link.zhihu.com/?target=https%3A//obsidian.md/)
* [英文社区/论坛/聊天室](https://link.zhihu.com/?target=https%3A//obsidian.md/community)
* [支持开发者](https://link.zhihu.com/?target=https%3A//obsidian.md/pricing)
* [图谱/双向链接软件大全](https://link.zhihu.com/?target=https%3A//www.notion.so/Artificial-Brain-Networked-notebook-app-a131b468fc6f43218fb8105430304709)

# 快速入门 

### 还不确定是否要使用obsidian?

推荐看下面的内容

* [从卡片链接到大脑联想，基于 Obsidian 的卡片盒笔记法实践](https://sspai.com/post/60802) ——吕立青_JimmyLv


### obsidian很棒！我要如何学习使用它？

推荐方法：看英文的使用手册（在[下载obsidian](https://obsidian.md)之后，可以通过左下角的问号`?`标识打开手册）

1. 看教学视频

* [https://youtu.be/gfAwa6wJqwA](https://youtu.be/gfAwa6wJqwA)
* [https://www.bilibili.com/video/BV1gK4y147M6](https://www.bilibili.com/video/BV1gK4y147M6)
* [https://www.bilibili.com/video/BV1xK4y147yJ](https://www.bilibili.com/video/BV1xK4y147yJ)

### 重新考虑用obsidian?

*列出劝退理由和可能的解决方案*

* 没有大纲：可以折迭
* 不是所见即所得：Ctrl + E 快速切换编辑和预览模式
* 无法精确引用：试试引用到标题 [[page#标题名称]]
# 软件比较

## obsidian优缺点

### **优点**

  * 支持双向链接、markdown
  * 有不少插件和可选配置，满足了不同用户的需求，有很多自定义设置，甚至还支持vim
  * 能够非常快速地在各种笔记之间跳转并快速创建链接（`ctrl+O`快捷键）
  * [社区](https://forum.obsidian.md/)很活跃

### **缺点(v0.7.3版本)**

  * 不支持[[大纲]]，但支持折迭（根据标题以及缩进）
    * 操作方法：通过设置，修改成支持”标题/缩进"的折迭。但预览preview中不支持，此外也没有记忆折迭（后面的版本会修复）。
  * 非云同步，需要借助dropbox git google drvie 坚果云之类
  * 无移动端/手机端
  * 没有TOC/目录功能（可以考虑用标签tag，#开发中）
  * 不支持typora式的所见即所得 #开发中 但需要很久
  * 暂时没有近义词/同义词alias功能
### **官方开发计划**[roadmap](https://trello.com/b/Psqfqp7I/obsidian-roadmap)

  * 已完成待发布：无
  * 正在开发：
    * 拼写检查
    * Graph视图以当前页为中心
    * Graph视图筛选
    * 搜索改进（匹配多个词语）
  * 短期计划：
    *  导出到标准 Markdown链接
    *  Obsidian同步Beta
    *  Obsidian发布版Beta
    *  插件 API Beta测试
  * 长期计划：
    * 编辑模式所见即所得（类似Typora）
    * 公共插件API（v1.0）
    * 移动端APP
## obsidian VS 其他软件 等等

*网友文章汇总*

* [比较Research，Obsidian，Remnote](https://zhuanlan.zhihu.com/p/149401362)
# FAQ

### markdown的语法？

见帮助手册中的[[format your code]]一节（按ctrl+O搜索/切换）。


### 为什么不支持[[大纲]]？

因为不需要大纲的人也有很多，obsidian基于markdown的文件格式难以实现，要改动底层代码（每一行当做一块处理）

不过obsidian支持[折](https://shimo.im/docs/H83hqTp9X9KqptVc#anchor-vRMQ)[迭](https://shimo.im/docs/H83hqTp9X9KqptVc#anchor-vRMQ)功能，可以解决部分需求

ps：obsidian的作者也是大纲软件dynalist的开发人员

### 为什么不做云同步？ 

笔记是一个很私人的东西，你应当掌握自己的数据，并决定自己的数据以何种方式做同步，无论是git、iCloud、Dropbox、坚果云还是其他方式

### markdown转pdf？

关于Markdown转PDF的方法

1. 使用Pandoc的包，具体可以在简书上寻找。或者参考：Markdown写作进阶：Pandoc入门浅谈，阳志平，[https://www.yang](https://www.yangzhiping.com/tech/pandoc.html)[zhiping.com/tech/pandoc](https://www.zettlr.com/)[.html](https://www.yangzhiping.com/tech/pandoc.html)。

2. 使用一些zk笔记软件，例如[zettlr](https://www.zettlr.com/)，里面内置了Pandoc程序。

# Obsidian进阶指南 / 使用技巧

### 常见技巧

* 想要高效利用obsidian，掌握快捷键吧！（在设置->快捷键中）
* `ctrl + alt + 左右键`返回/向前页面
* `![[obsidian]]`链接其他页面
* `$E=mc^2$`支持数学公式
* `[[]]`为内部page的链接方式，双方括号中填入page标题即可，外部链接方式为`[page](page link)`
* obsidian的缩进跟大纲的tab不大一样（但在设置中可以更改为和大纲一致）。
  * Indent        `Ctrl/Cmd ]`
  * Unindent      `Ctrl/Cmd [`

### link链接的高级用法

1. 可以用文件夹路径引用（这样就可以规避page同名的问题了）
  * [[project/知识管理/方法论]]
  * [[project/时间管理/方法论]]
1. [[Get things done|GTD]]，preview显示为GTD，链接到Get things done页面
1. [[Get things done#GTD原理]]，链接到Get things done页内标题“GTD原理”，达到块引用的效果。
1. [[Get things done#GTD原理|GTD]]，显示为GTD，实际链接到标题“GTD原理”
1. 还可以用相对路径，比如[[../方法论]]，指的是上一级目录里的“方法论”page
1. 还可以链接到本地的 [文件](file:///d:/docs/excel/body.csv) ，点击可以使用系统的应用启动该文件，不过0.7.3版本中，路径中不能有中文（开发者回应正在解决）。此外，路径中的空格要用“%20”替换。
1. 前面加感叹号  `![[主题]]` 即可在预览preview中看到引用的内容

# 知识管理方法论

### Zettelkasten

  * 阳志平，[构建优雅的知识创造系统](https://www.yangzhiping.com/psy/yang-KnowledgeSystem.html)
  * 少数派，[如何高效实践卡片式写作？](https://sspai.com/post/59109)
  * zettlr，[利用zotero和zettelkasten软件（比如obsidian）阅读和整理文献（回帖中有zettlr作者给出的详细图文教程，虽然是利用zettlr软件的，但是可以类比利用在obsidian上）](https://forum.zettlr.com/discussion/94/zotero-as-zettelkasten)
### PARA

  * [如何管理信息：P.A.R.A. 是什么及在 Notion 中的应用](https://mp.weixin.qq.com/s?__biz=MzAwOTUwNzI1Ng==&mid=2247483812&idx=1&sn=89414301b153d6165eb7feea9df1207b&chksm=9b5fd973ac285065f3a5308e0316307c816cca83535c765ab4b4a79b81e5cf6754e332dcf4ff&mpshare=1&scene=1&srcid=&sharer_sharetime=1591185871912&sharer_shareid=48387c294460ce9f025e4d1b2410155b&key=4b19ec3f0bdf89b5676b1fba422dd392a3d0dde3cb9345e70e3ffa387bda8a7ee43e1303d999f20a21289f8e6a97387d07f4cb68f8543679573c89751a966fb21c3f65da5aef7ad2e5ebe4c3a9667183&ascene=1&uin=MTM3MzQxNTcwMQ%3D%3D&devicetype=Windows+10+x64&version=62090070&lang=zh_CN&exportkey=Accu5yydsSknJ1Paf9dhTFA%3D&pass_ticket=RlK%2FIypGT1nB8oxcoayEAypJXKli9T812rNsS2DlbUMik1ofjwb5a7z099KeXoz8)
  * [P.A.R.A设计理念](https://www.notion.so/e0781dd14e87452eb8484ecc5f5636a9)
