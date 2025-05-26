---
tags:
  - type/structure
  - structure/reference
  - structure/list
  - target/starterkit
aliases: 
lead: +++ 引言段落放在这里 +++
created: 2023-04-02, 09:30
modified: 2025-03-30, 17:44
template_type: Structure
template_version: "1.4"
banner: "![[banner_books.jpg]]"
view_count: 1
---

# 词汇表

[[参考]] > [[作者]] | [[参考文献]] | [[书籍]] | [[词汇表]] | [[引言]]

<!-- DataView表格，用作示例并修改 -->
```dataview
TABLE WITHOUT ID
	file.link as 术语, 
	lead AS "定义",
	length(file.inlinks) as "引用"
FROM #type/term OR #type/tool 
WHERE lead != empty
SORT file.name ASC
```

## 无定义

<!-- DataView表格，用作示例并修改 -->
```dataview
TABLE WITHOUT ID
	file.link as 术语, 
	lead AS "定义",
	length(file.inlinks) as "引用"
FROM #type/term OR #type/tool 
WHERE lead = empty
SORT length(file.inlinks) DESC
```

## 仅工具

<!-- DataView表格，用作示例并修改 -->
```dataview
TABLE WITHOUT ID
	file.link as 术语, 
	lead AS "定义"
FROM #type/term AND #type/tool
SORT file.name ASC
```

## 卡片盒

<!-- DataView表格，用作示例并修改 -->
```dataview
TABLE WITHOUT ID
	file.link as 术语, 
	lead AS "定义"
FROM #type/term AND #theme/zettelkasten 
SORT file.name ASC
```
<!-- 选项 
TABLE WITHOUT ID
	file.folder AS ...
	file.link AS ...
	file.name AS ...
	file.etags AS ...

FROM #target/forumzettelkasten  : 使用标签时
FROM "Books"                                : 使用文件夹时
FROM ""                                          : 使用所有文件夹时
FROM #status/open OR #status/wip

SORT created DESC
SORT file.name ASC

WHERE read = 2023
WHERE status = "open"
WHERE contains(file.name,"LernOS Zettelkasten")

---
了解更多: 
https://github.com/blacksmithgu/obsidian-dataview/blob/master/docs/docs/queries/query-types.md
https://github.com/blacksmithgu/obsidian-dataview/blob/master/docs/docs/queries/data-commands.md

来源: 
https://github.com/groepl/Obsidian-Templates
-->


---
## 问题
<!-- 您还需要考虑什么？ --> 
- 


## 术语
<!-- 指向定义页面的链接 -->
- 


## 参考资料
<!-- 指向内容中未引用页面的链接 -->
- [草图笔记词汇表](Glossary%20of%20Sketchnotes.md)
- [卡片盒词汇表](Glossary%20of%20Zettelkasten.md)
- [PKM词汇表](PKM%20Glossary.md)
- https://blacksmithgu.github.io/obsidian-dataview/queries/dql-js-inline/ 用于"术语模板"
- 照片来自 [Maksym Kaharlytskyi](https://unsplash.com/@qwitka?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) 在 [Unsplash](https://unsplash.com/photos/Q9y3LRuuxmg?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)


