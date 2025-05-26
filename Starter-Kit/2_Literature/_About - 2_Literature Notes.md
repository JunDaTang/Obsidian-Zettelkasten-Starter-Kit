---
view_count: 2
created: 2024-07-26, 20:42
modified: 2025-03-30, 16:07
tags:
  - type/structure
  - structure/about
  - target/starterkit
aliases: 
lead: "**文献笔记**是对资料来源的总结，包含关键要点。它们从书籍、文章或讲座中提取有用的洞察。用于突出论点、总结理论和记录相关段落。"
visual: "![[image.jpg]]"
template_type: Structure
template_version: "1.14"
---
<!--  参见下方"模板帮助"了解属性使用方法 -->

<!--  清晰且描述性的标题 -->
![[About - 2_Literature Notes.canvas|关于 - 2_文献笔记]]
[[About - 1_Fleeting Notes|1_临时]] | [[_About - 2_Literature Notes|2_文献]] | [[_About - 3_Permanent Notes|3_永久]] | [[About - 4_Project Notes|4_项目]] | [[_About - 5_Structure Notes|5_结构]]

<!--  从属性部分的"lead"键中总结的结构  -->

> [!Definition]
> `= this.lead`

> [!Simple Rules]
>- 对决定保留的内容要极其有选择性。
>- 在来源的上下文中写作。
>- 始终保留指向来源的链接。

<!-- 我的内容的主要结构 -->
<!-- Dataview表格。用作示例并修改。 -->
```dataview
TABLE WITHOUT ID 
	file.link as "2_文献笔记", 
	(date(today) - file.cday).day as "存在天数" 
FROM "2_Literature"
SORT file.cday asc 
LIMIT 20
```


---
了解更多：[[Literature Notes]]
