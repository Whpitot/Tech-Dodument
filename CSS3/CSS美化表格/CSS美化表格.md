<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>CSS概述</title>
</head>
<body>
    <div>
		<strong>
			模块：CSS美化表格<br/>
			时间：2017-07-04<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>
	<div>
		<h5>表格基本样式</h5>
		<ul>表格边框样式
			<li><b>border</b>:
				<ul>
					<li><b>border-width</b>：规定边框的宽度</li>					
					<li><b>border-style</b>：规定边框的样式(solid double dotted dashed)</li>	
					<li><b>border-color</b>：规定边框的颜色</li>					
					<li><b>border-collapse</b>：表格的边框是否会合并为一个单一的边框</li>		
					<li><b>border-radius</b>：定义边框的圆角效果</li>					
				</ul>
			</li>
			<li><b>box-shadow</b>
				<ul>
					<li><b>X-offset</b>:阴影水平偏移量，如果值为正值，则阴影在对象的右边，其值为负值时，阴影在对象的左边；</li>
					<li><b>Y-offset</b>：阴影垂直偏移量，如果为正值，阴影在对象的底部，其值为负值时，阴影在对象的顶部；</li>
					<li><b>blur-radius</b>：阴影模糊半径，值越大，阴影边缘就越模糊；</li>
					<li><b>spread-radius</b>：阴影扩展半径，如果值为正，则整个阴影都延展扩大，反之值为负值时，则缩小；</li>
					<li><b>color</b>：阴影颜色，设置阴影颜色</li>
				</ul>
			</li>
		</ul>
		```
		border:1px solid green border-radius:10px border-collapse:separate
		```		
		<ul>表格背景颜色
			<li><b>background-color</b>：设置表格背景颜色，也可以设置表单元素背景颜色</li>
		</ul>
		```
			background-color:red
		```
	</div>
</body>
</html>