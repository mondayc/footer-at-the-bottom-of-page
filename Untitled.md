footer 固定在底部的若干方法
---
###两种情况：
- 页面内容未填充满时，footer 固定在底部；
- 页面填充满后，footer 随页面的增加填充在主体内容的下方

footer_1:

```
html,body{
	height: 100%;
}
*{
	margin: 0;
	padding: 0;
}
.container{
	min-height: 100%;
}
.content{
	padding-bottom: 30px;
	overflow: hidden;
}
.footer{
	margin-top: -30px;
	height: 30px;
	background-color: #eee;
}
/*
创建一个足够大的容器container 包含整个网页

并将footer 挤到底端，通过设置 margin-top = -30px 使footer 上浮

并在content 中设置padding-bottom 使之能容下页脚而不重叠
*/
```