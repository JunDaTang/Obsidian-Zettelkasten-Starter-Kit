---
view_count: 17
created: 2024-07-26, 20:42
modified: 2025-03-30, 16:06
tags:
  - type/structure
  - structure/about
  - target/starterkit
aliases: 
lead: "**临时笔记**是快速的想法或创意，具有临时性和非结构化特点。它们捕捉原始想法，防止遗失。用于记录自发的洞察、头脑风暴或初步反思。"
visual: "![[image.jpg]]"
template_type: Structure
template_version: "1.14"
---
<!--  参见下方"模板帮助"了解属性使用方法 -->


<!-- 可视化图表或草图（如果有的话） -->

![[About - 1_Fleeting Notes.canvas|关于 - 1_临时笔记]]
[[About - 1_Fleeting Notes|1_临时]] | [[_About - 2_Literature Notes|2_文献]] | [[_About - 3_Permanent Notes|3_永久]] | [[About - 4_Project Notes|4_项目]] | [[_About - 5_Structure Notes|5_结构]]


<!--  从属性部分的"lead"键中总结的结构  -->

> [!Definition]
> `= this.lead`

> [!Simple Rules]
> - 捕捉涌现在脑海中的想法。

<!-- 我的内容的主要结构 -->

<!-- Dataview表格。用作示例并修改。 -->
```dataview
TABLE WITHOUT ID 
	file.link as "1_临时笔记", 
	(date(today) - file.cday).day as "存在天数" 
FROM "1_Fleeting"
SORT file.cday asc 
```


---
了解更多：[[Fleeting Notes]]