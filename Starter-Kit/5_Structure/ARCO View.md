---
tags:
  - type/structure
  - structure/view
  - target/starterkit
aliases: ARCO
lead: 基于Nick Milo的ACE框架。
created: 2023-09-05, 16:04
modified: 2025-03-30, 16:36
template_type: Structure
template_version: "1.6"
banner: "![[IMG_0319.png]]"
banner_x: 0.5
view_count: 3
updated: 2024-10-23T17:47
---

[首页](Home.md) | [ARCO](ARCO%20View.md) |  [检查](Inspect%20View.md) 
<!-- 我的内容的主要结构 -->
> [!map]- 地图集
> _地图册_
>
>[[地图集]] > [[工作]] | [[社区]] | [[家庭]] | [[自我]] 
> 

> [!reference]- 参考
> _事实和外部链接册_
>
> [[参考]] > [作者](Authors.md) | [参考文献](Bibliography.md) | [书籍](Books.md) | [词汇表](Glossary.md) | [引言](Quotes.md)

> [!calendar]- 日历
> _事件册_
>
>###### 会议
>- [[卡片盒圆桌 - 周一]] | [WOL Troy - 周五](WOL%20Circle%202024.md)
>
>###### 子弹日记
>
>- [2023](2023.md) | [2024](2024.md) | [[2025]]
>- [[2025年1月]] | [[2025年2月]] | [[2025年3月]]
>- [[子弹日记收集]]
>
>###### 目标与关键结果
>- [[2022年OKR]] | [[2023年OKR]] | [[2024年OKR]] | [[2025年OKR]]
>
>###### 愿景板
>- [[2022年愿景板]] | [2023年愿景板](Vision%20Board%202023.md) | [[2024年愿景板]]
>- [[2022年愿望]] | 
>- [[想法列表]] | 

> [!organizer]- 组织者
> _任务和项目册_
>
> ###### 项目
> [_e1 - 做有用的笔记](_e1%20-%20Make%20Useful%20Notes.md) | [LinkedIn](LinkedIn%20Log.md)
> 
> ###### 任务
> [任务](Tasks.md) |  [待办任务](Tasks%20Open.md) | [来自电子书](Tasks%20from%20E-book.md) | [来自卡片盒](Tasks%20-%20Zettelkasten.md) | [来自草图笔记](Tasks%20-%20Sketchnotes.md)
> 
> ###### 看板
> [看板](Kanban%20Board.md) | [看板仪表板](Kanban%20Dashboard.canvas)
>
>> [!backlog]- 待办事项
>>```dataview
>>TABLE WITHOUT ID
>>	file.link as 笔记,
>>	file.cday AS "创建时间", 
>>	file.folder AS "文件夹" 
>>FROM "" 
>>WHERE kanban = "backlog"
>>SORT file.folder ASC
>>```
>
>>[!todo]- 待做
>>```dataview
>>TABLE WITHOUT ID
>>	file.link as 笔记,
>>	file.cday AS "创建时间", 
>>	file.folder AS "文件夹" 
>>FROM "" 
>>WHERE kanban = "todo"
>>SORT file.folder ASC
>>```
>
>>[!doing]+ 进行中 - _WIP限制3个_
>>```dataview
>>TABLE WITHOUT ID
>>	file.link as 笔记,
>>	file.cday AS "创建时间", 
>>	file.folder AS "文件夹" 
>>FROM "" 
>>WHERE kanban = "doing"
>>SORT file.folder ASC
>>```
>
>>[!done]- 已完成
>>```dataview
>>TABLE WITHOUT ID
>>	file.link as 笔记,
>>	file.mday AS "修改时间", 
>>	file.folder AS "文件夹" 
>>FROM "" 
>>WHERE kanban = "done"
>>SORT file.mday DESC
>>LIMIT 5
>>```
>

<small>*) 100%有机思维。少于5%的AI生成想法。</small>