<!-- 随机引言的DataviewJS。用作示例并修改 -->
> [!QUOTE]
> ```dataviewjs 
> // 引言列表 
> let quotes = []; 
>
> // 从页面中提取引言
> dv.pages("#theme/zettelkasten") 
>	.where(page => page.quote) 
>	.forEach(page => { 
>		dv.array(page.quote) 
>			.forEach(quote => { quotes.push({ 
>				message: (quote), 
>				page: page }); 
>	})}); 
>
> // 选择随机引言
> let text = quotes[Math.floor(Math.random() * quotes.length)] 
>
> // 生成带引言的文本
> dv.paragraph(text.message + " <br>- " 
>	+ text.page.author + " <br><br><small>来自: " 
>	+ text.page.file.link) + "</small>"; 
> ```
<!-- 
引言按标签过滤。在此示例中：#theme/zettelkasten。如需要请修改脚本。
前言中的必需属性："quote"和"author"。
-->