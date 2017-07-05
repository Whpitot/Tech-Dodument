<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>CSS概述</title>
</head>
<body>
    <div>
		<strong>
			模块：CSS美化背景<br/>
			时间：2017-07-05<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>
	<div>
		<h5>背景相关竖向</h5>
		<ul>
			<li><b>background-color</b>：背景颜色 默认值：transparent</li>
			<li><b>background-image</b>：指定要使用的一个或多个背景图像 默认值：none</li>
			<li><b>background-repeat</b>：指定如何重复背景图像 默认值：repeat
				<ul>
					<li><b>repeat</b> 在横向和纵向上平铺</li>
					<li><b>no-repeat</b> 不平铺</li>
					<li><b>repeat-x</b> 在横向上平铺</li>
					<li><b>repeat-y</b>	在纵向上平铺</li>
				</ul>
			</li>
			<li><b>background-attachment</b>设置背景图像是否固定或者随着页面的其余部分滚动 默认值:scroll
				<ul>
					<li><b>scroll</b>跟随内容滚动</li>
					<li><b>fixed</b> 不论怎样滚动,始终固定在页面上</li>
				</ul>
			</li>
			<li><b>background-position</b>：	指定背景图像的位置 默认值：默认值:0% 0%
				<ul>
					<li><b>background-position: length || length</b></li>
					<li><b>background-position: position || position</b></li>
				</ul>
			</li>
		</ul>	
	</div>
</body>
</html>