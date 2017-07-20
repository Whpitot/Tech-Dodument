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
			<li><b>background-size</b>：	指定背景图像的大小
				<ul>
					<li><b>auto</b>：默认值，保持图片原来的大小 </li>
					<li><b>length</b>:表示具体的值，第一个值表示宽度，第二值表示高度；如果只给出一个值，第二个只自动为auto</li>
					<li><b>percentage</b>:表示百分比，用法同上</li>
					<li><b>cover</b>:此值是将图片放大，以适合铺满整个容器；适合于图片大小小于容器的情况</li>
					<li><b>contain</b>:此值是将图片放大，以适合铺满整个容器；适合于图片大于容器的情况</li>
				</ul>
			</li>
			<li><b>Transform</b>：Transform属性应用于元素的2D或3D转换。这个属性允许你将元素旋转，缩放，移动，倾斜等
				<ul>
					<li><b>translate(X,Y)</b>：表示水平、垂直移动该元素块</li>
					`transform:translate(120,120) 表示向右位移120px，如果向上位移120px`
					<li><b></b>：</li>
				</ul>
			</li>
		</ul>	
	</div>
</body>
</html>