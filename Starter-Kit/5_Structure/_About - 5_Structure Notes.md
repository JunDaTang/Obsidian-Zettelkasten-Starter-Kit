---
tags:
  - type/structure
  - structure/list
  - theme/zettelkasten
  - target/starterkit
aliases: 
lead: "**结构笔记**是高层次的笔记，将相关笔记组织并连接成有意义的结构。它们作为笔记集群的_索引中心_，指导相关想法的导航。用于创建关键主题的概览、将相关概念链接在一起，以及映射想法之间的关系。"
created: 2024-08-19, 13:36
modified: 2025-03-30, 16:36
template_type: Structure
template_version: "1.14"
view_count: 2
---
<!--  参见下方"模板帮助"了解属性使用方法 -->

![[About - 5_Structure Notes.canvas|关于 - 5_结构笔记]]
[[About - 1_Fleeting Notes|1_临时]] | [[_About - 2_Literature Notes|2_文献]] | [[_About - 3_Permanent Notes|3_永久]] | [[About - 4_Project Notes|4_项目]] | [[_About - 5_Structure Notes|5_结构]]

<!--  从属性部分的"lead"键中总结的结构  -->

> [!Definition]
> `= this.lead`



<!-- 我的内容的主要结构 -->

```dataview
TABLE WITHOUT ID 
	file.link as "5_结构笔记", 
	(date(today) - file.cday).day as "存在天数",
	view_count AS "打开次数"
FROM "5_Structure"
SORT file.cday desc
LIMIT 20
```

---
了解更多：[[结构笔记]]

