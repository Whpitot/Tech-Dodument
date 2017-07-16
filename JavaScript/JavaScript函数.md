<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>html5中使用CSS的方法</title>
</head>
<body>
    <div>
		<strong>
			模块：函数<br/>
			时间：2017-07-09<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>	
	<div>
		<h5>函数简介</h5>
		<p style="text-indent:2em">
		在程序设计中，可以将一段经常使用的代码封装起来，在需要的时候直接调用，这种封装叫函数；
		<ul>函数分类
			<li>按参数个数划分：有参函数和无参函数</li>
			<li>按返回值划分：有返回值函数和无返回值函数</li>
			<li>按编写函数的对象划分：预定义函数（系统函数）和自定义函数</li>
		</ul>
		<p>	
	</div>
	<div>
		<h5>定义函数</h5>
		<p>定义函数的关键字：Function</p>
		<ul>
			<li>不指定函数名</li>
			`function([参数1，参数2]) { //函数体语句 } `
				<ul>
					<li>把函数直接赋给变量</li>
					`var myFun  = function([参数1，参数2]) { //函数体语句 } `
					<li>网页事件直接调用函数</li>
					`window.onload = function([参数1，参数2]) { //函数体语句 } `
				</ul>
			<li>指定函数名</li>
			可带函数的返回值 Return
			`function 函数名 ([参数1，参数2]) { //函数体语句  [return 表达式]} `
		</ul>
	</div>
	<div>
		<h5>调用函数</h5>
		<ul>
			<li>直接调用</li>
			`函数名([参数1……])`  
			`calcF(inValue)`
			<li>在表达式调用</li>
			`var myFun  = calcF(inValue) `
			<li>在事件中调用</li>
			`window.onload = calcF(inValue) `
		</ul>
	</div>
	<div>
		<h5>系统函数</h5>
		<ul>
			<li><b>Eval(字符串)</b>：计算JavaScript字符串、并把它作为脚本代码执行</li>
			<li><b>isNaN(参数)</b>：检查某个值是否为数字</li>
		</ul>
	</div>
</body>
</html>