---
tags:
  - type/structure
  - structure/moc
  - structure/index
  - target/project
  - target/github
  - target/starterkit
aliases: 
created: 2023-11-21, 20:38
modified: 2025-03-30, 16:03
banner: "![[IMG_0319.png]]"
banner_x: 0.5
lead: 卡片盒起始页。必要时可修订。
visual: "![[image.jpg]]"
template_type: Structure
template_version: "1.12"
view_count: 185
---
[首页](Home.md) | [ARCO](ARCO%20View.md) |  [检查](Inspect%20View.md)

```dataviewjs
// 选择随机引言或想法
let a = Math.random()

if (a < 0.5) {

dv.paragraph(">[!Quote]")

// 引言列表
let quotes = []; 

// 从页面中提取引言
dv.pages() 
	.where(page => page.quote) 	.forEach(page => { 
		dv.array(page.quote) 
			.forEach(quote => { quotes.push({ 
				message: (quote), 
				page: page }); 
	})}); 

// 选择随机引言
let text = quotes[Math.floor(Math.random() * quotes.length)] 

dv.paragraph("> " + text.message + " <br>- " 
	+ text.page.author + " <br><br><small>来源: " 
	+ text.page.file.link) + "</small>"; 

} else {
 
 dv.paragraph(">[!Remember]-")
 // 想法列表
 let ideas = []; 

 // 从页面中提取想法
 dv.pages('"3_Permanent" AND #theme/zettelkasten') 
	.where(page => page.lead) 
	.forEach(page => { 
		dv.array(page.lead) 
			.forEach(lead => { ideas.push({ 
				message: (lead), 
				page: page }); 
	})}); 

 // 选择随机想法
 let text = ideas[Math.floor(Math.random() * ideas.length)] 

 dv.paragraph("> " +
 	"<b>" + text.page.file.name + "</b><br>" +
 	text.message + 
 	" <br><br><small>" + 
 	text.page.file.link +  " - " +
 	text.page.template_type  + ", " +
 	text.page.file.inlinks.length  + " 入链, " +
 	text.page.file.outlinks.length  + " 出链, " +
 	text.page.file.etags.length  + " 标签, " +
 	text.page.file.tasks.length  + " 任务, " +
 	moment(text.page.file.cday.toString()).format("DD.MM.YYYY") + "." +
 	"</small>"
 	);
 } 
```

`<small>`*) 100% 有机思维。少于5%的AI生成想法。`</small>`
