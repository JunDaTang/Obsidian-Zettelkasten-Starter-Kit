---
tags:
  - type/structure
  - structure/list
  - target/starterkit
banner: "![[banner_books.jpg]]"
created: 2022-03-04, 19:32
modified: 2025-03-30, 16:54
view_count: 1
template_type: Structure
---
  
# 书籍 
<!-- 用于进一步学习或作者参考的书籍列表。  -->
[[参考]] > [[作者]] | [[参考文献]] | [[书籍]] | [[词汇表]] | [[引言]]

> [[书籍地图]]

### 正在阅读
```dataview 
TABLE WITHOUT ID
	bibliography AS "书籍",
	file.link as 笔记
From #type/book 
Where contains(status, "reading") 
SORT bibliography ASC
```  

### 芝加哥第17版格式参考文献
```dataview
TABLE WITHOUT ID
	bibliography AS "书籍",
	file.link as 笔记
FROM #type/book
WHERE bibliography !=empty
SORT file.name ASC
```

### 草图笔记书籍

```dataview
TABLE WITHOUT ID
	bibliography AS "书籍",
	file.link as 书籍
FROM #type/book and #theme/sketchnotes 
SORT file.name ASC
```

### 卡片盒书籍

```dataview
TABLE WITHOUT ID
	bibliography AS "书籍",
	file.link as 书籍
FROM #type/book and #theme/zettelkasten  
SORT file.name ASC
```

### 其他书籍

```dataview
TABLE WITHOUT ID
	file.link as 书籍, 
	file.mday AS "修改时间", 
	file.folder AS "文件夹" 
FROM #type/book and !#theme/sketchnotes and !#theme/zettelkasten
SORT file.name ASC
```


___

- 芝加哥格式手册第17版（注释）
- 搜索参考文献数据：[https://zbib.org](https://zbib.org/)

Zotero Bib
https://zbib.org/2f8ce7173dee4e32a4efe1f6312395b6

28.03.2022
https://zbib.org/57974b2429a84839be10d1f03cf13681

导出选项：
- 保存到Zotero
- 下载BibTeX
- 下载RIS

___


##### 参考资料
- _照片来自 <a href="https://unsplash.com/@chuttersnap?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">CHUTTERSNAP</a> 在 <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>_
- [阅读列表](List%20of%20Reading.md)

### 按引用链接排序的书籍

```dataview
TABLE WITHOUT ID
	file.link as 书籍, 
	length(file.inlinks) AS 引用,
	file.mday AS "修改时间", 
	file.folder AS "文件夹" 
FROM #type/book
SORT length(file.inlinks) DESC
```
