---
view_count: 2
created: 2024-08-19, 13:37
modified: 2025-03-30, 16:36
tags:
  - type/structure
  - structure/canvas
  - target/starterkit
aliases: 
lead: "**项目笔记**是与特定、有时限的项目相关的笔记，包含可执行的任务、研究和草稿。它们将临时的、目标导向的信息与永久知识分开。用于管理文章研究、跟踪书籍进度或组织演示材料。"
visual: "![[image.jpg]]"
template_type: Structure
template_version: "1.14"
---
<!--  参见下方"模板帮助"了解属性使用方法 -->

![[About - 4_Project Notes.canvas|关于 - 4_项目笔记]]
[[About - 1_Fleeting Notes|1_临时]] | [[_About - 2_Literature Notes|2_文献]] | [[_About - 3_Permanent Notes|3_永久]] | [[About - 4_Project Notes|4_项目]] | [[_About - 5_Structure Notes|5_结构]]

<!-- 如果有的话，视觉或草图笔记 -->

<!--  从属性部分的"lead"键中总结的结构  -->

> [!Definition]
> `= this.lead`

> [!Simple Rules]
>- 一个项目，一个文件夹。
>- 始终保留指向来源的链接。
>- 添加指向目标的链接。

<!-- 我的内容的主要结构 -->

---
[[Obsidian论坛]] | [[卡片盒论坛]] | [[About - 4_Project Notes|6_项目笔记]]

```dataview
TABLE WITHOUT ID 
	file.link as "5_项目笔记", 
	visual as 视觉,
	target as 目标,
	(date(today) - file.cday).day as "存在天数" 
FROM "4_Project"
SORT file.cday desc
LIMIT 30
```

---
了解更多：[[项目笔记]]
