---
view_count: 1
created: 2025-03-30, 16:01
modified: 2025-03-30, 18:11
tags:
  - type/structure
  - structure/moc
  - target/starterkit
aliases: 
lead: 在GitHub上发布的Obsidian启动套件的笔记列表。
template_type: Structure
template_version: "1.18"
---
<!--  参见下方"模板帮助"了解属性使用方法 -->

# MOC - Obsidian启动套件
<!--  清晰且描述性的标题 -->

<!--  从属性部分的"lead"键中总结的结构  -->

> [!Note]
> `= this.lead`

<!-- 我的内容的主要结构 -->

<!-- Dataview表格。用作示例并修改。 -->

```dataview
TABLE 
	rows.file.link AS 笔记,
	rows.template_type AS 模板,
	dateformat(rows.file.mday, "yyyy-LL-dd") AS 修改时间
FROM #target/starterkit 
FLATTEN file.folder
GROUP BY file.folder AS 文件夹
SORT 文件夹 ASC
SORT 笔记 ASC
```


---
# 后附内容

**来源**
<!-- 始终保留指向来源的链接- --> 
- based_on:: [GROUP BY查询示例 - Dataview示例库](https://s-blu.github.io/obsidian_dataview_example_vault/20%20Dataview%20Queries/Example%20GROUP%20BY%20Queries/)

**参考资料**
<!-- 指向内容中未引用页面的链接。参见: [[相关笔记]] 因为 <原因> -->
- see:: 

**术语**
<!-- 指向定义页面的链接。 -->
- 

**目标**
<!-- 指向项目笔记或外部发布内容的链接。 -->
- used_in::

---
**任务**
<!-- 这个笔记还需要做什么？ --> 
- 

**问题**
<!-- 您还需要考虑什么？ --> 
- question::

---
**模板帮助**
<!-- 指向GitHub上外部帮助页面的链接。 -->
- [基本模板结构](https://github.com/groepl/Obsidian-Templates#basic-template-structure)
- [如何使用链接](https://github.com/groepl/Obsidian-Templates#how-to-use-links)
- [如何使用标签](https://github.com/groepl/Obsidian-Templates#how-to-use-tags)
- [如何搜索笔记](https://github.com/groepl/Obsidian-Templates#how-to-search-notes)
- [所需插件](https://github.com/groepl/Obsidian-Templates#obsidian-plugins-needed)
- [查找最新更新](https://github.com/groepl/Obsidian-Templates)