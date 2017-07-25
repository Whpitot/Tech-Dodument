<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>html5中使用CSS的方法</title>
</head>
<body>
    <div>
		<strong>
			模块：CSS选择器<br/>
			创建时间：2017-07-03<br/>
			修改时间：2017-07-25<br/>
			编写人：小帅<br/>
			版本：V1.1						
		</strong>
	</div>
	<hr/>	
	<div>
		<h6>CSS选择器</h6>	
		<ul>
			<li><b>说明：</b>通过不同的CSS选择器可以控制html中的每个标记，从而达到控制整个html文档的呈现样式</li>
			<li><b>分类</b>
				<ul>
					<li><b>基础选择器</b></li>
					<li><b>层次选择器</b></li>
					<li><b>伪类选择器</b></li>					
					<li><b>伪元素</b></li>
					<li><b>属性选择器</b></li>
				</ul>
			</li>			
		</ul>
	</div>
	<hr/>
	<div>
		<h5>基础选择器</h5>	
		<ul>
			<li><b>* ---- 通配选择器</b>：选择文档中所以HTML元素</li>
			`* { margin:0; padding:0; }`  
			<li><b>E ---- 元素选择器</b>：选择指定类型的HTML元素</li>
			`p { font-size:2em; }`   
			`<p>css选择器</p>`
			<li><b>#id ---- ID选择器</b>：选择指定ID属性值为“id”的任意类型元素</li>
			`#info { background:#ff0; }`  
			`<p id="info">css选择器</p>` 
			<li><b>.class ---- 类选择器</b>：选择指定class属性值为“class”的任意类型的任意多个元素</li>
			`.info { background:#ff0; }` 
			`<p class="info">css选择器</p>`
			<li><b>.class1.class2 ---- 多类选择器</b>：选择指定class属性为“class1 class2”的元素</li>
			`.info1.info2 { background:#ff0; }`
			 `<p id="info1 info2">css选择器</p>`  	
		</ul>				  
	</div>
	<hr/>
	<div>
		<h5>层次选择器</h5>	
		<ul>
			<li><b>E F ---- 后代元素选择器</b>：匹配所有属于E元素后代的F元素，E和F之间用空格分隔</li>
			`p span{ background:#ff0; }`  
			`<p>`  
				`<span>css选择器</span>`  
			`</p>`  
			<li><b>E,F ---- 多元素选择器</b>：同时匹配所有E元素或F元素，E和F之间用逗号分隔</li>
			`h1,h2,h3,h4,h5,h6 { background:#ff0; }`  
			`<h1>css选择器</h1>`  
			`<h2>css选择器</h2>`
			<li><b>	E>F ---- 子元素选择器</b>：匹配所有E元素的子元素F</li>
			`p > span{ background:#ff0; }`  
			`<p>`  
				`<span>css选择器</span>`  
			`</p>`  
			<li><b>E+F ---- 毗邻元素选择器</b>：匹配所有紧随E元素之后的同级元素F</li>
			`p + span{ background:#ff0; }`  
			`<p>`  
				`<span>css选择器</span>`  
			`</p>`  
		</ul>		
	</div>
	<hr/>
	<div>
		<h5>伪类选择器</h5>	
		<ul>
			<li style="font-style:oblique"><b>动态伪类选择器</b></li>
			<li style="font-style:oblique"><b>目标伪类选择器</b></li>
			<li style="font-style:oblique"><b>语言伪类选择器</b></li>
			<li style="font-style:oblique"><b>UI元素状态伪类选择器</b></li>
			<li style="font-style:oblique"><b>结构伪类选择器</b></li>
			<li style="font-style:oblique"><b>否定伪类选择器</b></li>
		</ul>
		<h5>动态伪类选择器</h5>
		<ul>
			<li><b>E:hover</b>：匹配鼠标悬停其上的E元素</li>
			<li><b>E:focus</b>：匹配获得当前焦点的E元素</li>
		</ul>
		<h5>目标伪类选择器</h5>
		<ul>
			<li><b>E:target</b>：匹配文档中特定"id"点击后的效果</li>			
		</ul>
		<h5>结构伪类选择器</h5>
		<ul>
			<li><b>E:fisrt-child</b>：父元素E的第一个子元素。与E:nth-child(1)等同</li>
			<li><b>E:last-child</b>：父元素的最后一个子元素,与E:nth-last-child(1)</li>
		</ul>
	</div>
	<hr/>
	<div>
		<h5>属性选择器</h5>
		<ul>
			<li><b>E[att^="val"]</b>：属性att的值以"val"开头的元素</li>
			<li><b>E[att$="val"]</b>：属性att的值以"val"结尾的元素</li>
			<li><b>E[att*="val"]</b>：属性att的值包含"val"字符串的元素</li>
		</ul>
			```
			div[id^ ="val"]{ background:#ff0; }
			```
	</div>
</body>
<html>