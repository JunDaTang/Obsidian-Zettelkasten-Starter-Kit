---
tags:
  - structure/list
  - structure/index
  - type/dataview
  - type/project
  - target/starterkit
banner: "![[banner_books.jpg]]"
created: 2022-03-04, 19:32
modified: 2025-03-30, 16:57
template_type: Structure
view_count: 1
---
  
# 引言
<!-- 来自著名作者的引言列表  -->
[[参考]] > [[作者]] | [[参考文献]] | [[书籍]] | [[索引列表|索引]] | [[词汇表]] | [[引言]]

### 数据故事
```dataview
TABLE WITHOUT ID
	author AS 作者, 
	quote AS 引言, 
	file.link as 文件
FROM #type/quote and 
	#theme/datastory  
SORT author ASC
```

### 学习
```dataview
TABLE WITHOUT ID
	author AS 作者, 
	quote AS 引言, 
	file.link as 文件
FROM #type/quote and 
	#theme/learning 
SORT author ASC
```

### 草图笔记

```dataview
TABLE WITHOUT ID
	author AS 作者, 
	quote AS 引言, 
	file.link as 文件
FROM #type/quote and 
	#theme/sketchnotes 
SORT author ASC
```

### 思维

```dataview
TABLE WITHOUT ID
	author AS 作者, 
	quote AS 引言, 
	file.link as 文件
FROM #type/quote and 
	#theme/thinking   
SORT author ASC
```

### 写作

```dataview
TABLE WITHOUT ID
	author AS 作者, 
	quote AS 引言, 
	file.link as 文件
FROM #type/quote and 
	#theme/writing   
SORT author ASC
```

### 卡片盒
```dataview
TABLE WITHOUT ID
	author AS 作者, 
	quote AS 引言, 
	file.link as 文件
FROM #type/quote and 
	#theme/zettelkasten  
SORT author ASC
```




### 其他引言

```dataview
TABLE WITHOUT ID
	author AS 作者, 
	quote AS 引言,
	file.link AS 文件
FROM #type/quote and !#theme/sketchnotes and !#theme/zettelkasten AND !#theme/writing AND !#theme/datastory AND !#theme/thinking AND !#theme/learning
WHERE quote != empty
SORT author ASC
```

### 无作者引言
```dataview
TABLE WITHOUT ID
	author AS 作者, 
	quote AS 引言,
	file.link AS 文件
FROM #type/quote and 
	!#theme/sketchnotes AND
	!#theme/zettelkasten AND 
	!#theme/writing
WHERE quote = empty
SORT author ASC
```

## 参考资料
- _照片来自 <a href="https://unsplash.com/@chuttersnap?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">CHUTTERSNAP</a> 在 <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>_
- 使用[[Obsidian插件 - Dataview]]查询
