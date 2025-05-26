---
tags:
  - type/structure
  - theme/zettelkasten
  - structure/about
  - target/starterkit
aliases: 
lead: "**永久笔记**是经过处理的、独立的洞察，有意义地链接到系统中。它们将临时想法转化为可以重新访问和构建的结构化知识。用于用自己的话写笔记，将它们链接到相关概念，并使它们可重复使用。"
visual: "![[image.jpg]]"
created: 2024-07-28, 13:49
modified: 2025-03-30, 16:36
template_type: Structure
template_version: "1.14"
view_count: 2
---
<!--  参见下方"模板帮助"了解属性使用方法 -->

<!--  清晰且描述性的标题 -->

<!-- 如果有的话，视觉或草图笔记 -->

![[About - 3_Permanent Notes.canvas|关于 - 3_永久笔记]]
[[About - 1_Fleeting Notes|1_临时]] | [[_About - 2_Literature Notes|2_文献]] | [[_About - 3_Permanent Notes|3_永久]] | [[About - 4_Project Notes|4_项目]] | [[_About - 5_Structure Notes|5_结构]]

<!--  从属性部分的"lead"键中总结的结构  -->

> [!Definition]
> `= this.lead`

> [!Simple Rules]
>- 对决定保留的内容要极其有选择性。
>- 使用独特且描述性的标题。
>- 使用自己的话。
>- 不要在一个笔记中混合多个想法。
>- 一个想法，一个笔记。
>- 用三句话或更少的话总结笔记的主要想法。
>- 留下重新访问想法的理由。
>- 始终保留指向来源的链接。

<!-- 我的内容的主要结构 -->
```dataview
TABLE WITHOUT ID 
	file.link as "3_永久笔记", 
	(date(today) - file.cday).day as "存在天数",
	view_count AS "打开次数"
FROM "3_Permanent"
SORT file.cday desc
LIMIT 20
```


---
了解更多：[[永久笔记]]


