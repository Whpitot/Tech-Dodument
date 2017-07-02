<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>CSS概述</title>
</head>
<body>
    <div>
		<strong>
			模块：CSS3字体和段落属性<br/>
			时间：2017-07-03<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>
	<div>
		<h6>字体属性</h6>
		<ul>
			<li><b>font-family：</b>用于指定文字字体类型，如宋体、黑体、Times New Roman</li>
			```
			<p style="font-family:华文彩体、黑体、宋体">天行健，君子以自强不息</p>
			```
			<li><b>font-size：</b>设置字体大小</li>
			```
			<p style="font-size:10pt">天行健，君子以自强不息</p>
			```
			<li><b>font-style：</b>定义字体风格、及字体的显示样式
				<ul>
					<li><b>normal:</b>默认值，标准的字体样式</li>
					<li><b>italic:</b>斜体的字体样式</li>
					<li><b>oblique:</b>倾斜的字体样式</li>
					<li><b>inherit:</b>从父元素继承的字体样式</li>
				</ul>
			</li>
			```
			<p style="font-style:italic">天行健，君子以自强不息</p>
			```
			<li><b>font-weight:</b>定义字体的粗细程度
				<ul>
					<li><b>normal:</b>标准字体</li>
					<li><b>bold:</b>定义粗体字体</li>
					<li><b>bolder:</b>定义更粗的字体、相对值</li>
					<li><b>lighter:</b>定义更细的字体、相对值</li>
				</ul>			
			</li>
			```
			<p style="font-weight:bold">天行健，君子以自强不息</p>
			```
			<li><b>color: </b>定义字体颜色
				<ul>
					<li><b>color_name: </b>属性值为颜色名称 (red)</li>
					<li><b>hex_number: </b>属性值为十六进制的颜色 (#ff0000)</li>
					<li><b>rgb_number: </b>属性值为rgb代码的颜色 (rgb(255,0,0))</li>
					<li><b>inherit: </b>从父元素继承颜色</li>
				</ul>
			</li>
			```
			<p style="color:red">天行健，君子以自强不息</p>
			```
			<li><b>字体符合属性font</b></li>
			```
			{font:font-style font-variant font-weight font-size font-family}
			{font:nomal small-caps bold 20pt 宋体,"Times New Roman"}
            ```						
		</ul>
	</div>
</body>
</html>
