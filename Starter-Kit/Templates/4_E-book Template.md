---
tags: 
- type/chapter 
- theme/xyz
- target/ebook 
aliases:
visual: "![[IMGAGE.png]]"
title_short: "e1"
rule: +++ 在这里添加简单规则 +++
chapter: "0.0"
version: "0.1"
book_version: 0.19
status: draft
word_count: 0
bar: <progress max=100 value=0></progress><br>0% 初步想法
created: {{DATE:YYYY-MM-DD, HH:mm}}
modified: {{DATE:YYYY-MM-DD, HH:mm}}
published:
views: 0
feedbacks: 0
template_type: Ebook
template_version: "1.26"
---
<!--  
status: draft, final, published, revised 
bar: <progress max=100 value=0></progress><br>0% 初步想法 
	10% 承诺收获, 20% 用于教学, 30% 提供价值  
	40% 前置价值, 50% 高页面价值, 60% 价值测试
	70% 收到反馈, 80% 价值改进, 90% 最终润色, 100% 推荐 
-->

# {{Title}} - e1
<!--  清晰且描述性的标题 -->

```dataviewjs 
var progress_bar = (dv.current().bar);
var note_status = (dv.current().status);
dv.paragraph(progress_bar + ', ' + note_status);
```

<!-- 如果有的话，我的草图笔记 -->
```dataviewjs 
dv.paragraph(dv.current().visual);
```

<!-- 如果有的话，激励性引言 -->

<!-- 本章的主要内容 -->

<!-- 要记住的简单规则  -->
```dataviewjs 
dv.paragraph('> ' + dv.current().rule);
```

<!-- 脚注中的参考资料  -->


---
# 后附内容

**来源**
<!-- 始终保留指向来源的链接- --> 
- based_on::

**任务**
<!-- 获得最终版本还需要做什么？如果与流程相关，使用看板。 --> 
- 

**反馈**
<!-- 在草稿版本中您还需要考虑什么？ --> 
**0.14**
- 

**目录**
<!-- 指向电子书章节的链接 -->
- [004 - 目录](004%20-%20Contents.md)


**参考资料**
<!-- 指向内容中未引用页面的链接。参见: [[相关笔记]] 因为 <原因> -->
- see::
- 

**目标**
- target::

**模板帮助**
<!-- 指向GitHub上外部帮助页面的链接。 -->
- [基本模板结构](https://github.com/groepl/Obsidian-Templates#basic-template-structure)
- [如何使用链接](https://github.com/groepl/Obsidian-Templates#how-to-use-links)
- [如何使用标签](https://github.com/groepl/Obsidian-Templates#how-to-use-tags)
- [如何搜索笔记](https://github.com/groepl/Obsidian-Templates#how-to-search-notes)
- [所需插件](https://github.com/groepl/Obsidian-Templates#obsidian-plugins-needed)
- [查找最新更新](https://github.com/groepl/Obsidian-Templates)

