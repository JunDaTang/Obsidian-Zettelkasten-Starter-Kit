<!-- Dataview表格。用作示例并修改。 -->
```dataview
TABLE WITHOUT ID
	file.link as 书籍, 
	read AS "阅读", 
	created AS "创建", 
	file.folder AS "文件夹" 
FROM #type/book
SORT file.name ASC
WHERE read = 2022
LIMIT 5
```

<!-- 选项 
TABLE WITHOUT ID
	file.folder AS ...
	file.link AS ...
	file.name AS ...
	file.etags AS ...
	length(file.outlinks) AS …
	length(file.inlinks) AS …
	length(file.etags) AS …
	dateformat(file.cday, "yyyy-MM-dd") AS Date
	dateformat(file.cday, "yyyy-LLL-dd") AS Date
	dateformat(date(created, "yyyy-mm-dd, HH:MM"), "yyyy-mm-dd") AS "created" ⚡️DataView中的错误 


FROM #target/forumzettelkasten  : 使用标签时
FROM "Books"                                : 使用文件夹时
FROM ""                                          : 使用所有文件夹时
FROM #status/open OR #status/wip

GROUP BY author

SORT created DESC
SORT file.name ASC

WHERE read = 2023
WHERE status = "open"
WHERE kanban = "backlog"
WHERE contains(file.name,"LernOS Zettelkasten")
WHERE sketchnote != empty

LIMIT 3

---
了解更多: 
https://github.com/blacksmithgu/obsidian-dataview/blob/master/docs/docs/queries/query-types.md
https://github.com/blacksmithgu/obsidian-dataview/blob/master/docs/docs/queries/data-commands.md

来源: 
https://github.com/groepl/Obsidian-Templates
-->
