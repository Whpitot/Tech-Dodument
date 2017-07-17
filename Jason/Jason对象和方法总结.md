<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>CSS概述</title>
</head>
<body>
    <div>
		<strong>
			模块：JsonConvert<br/>
			时间：2017-07-14<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>
	<div>
	<p style="text-indent:2em">
		写在前面：关注一个对象主要关注他的程序集(怎样去找到这个对象)，构造函数(怎样去构造一个对象),</br>
		主要的属性和方法(怎样去使用这个对象);
	</p>
	</div>
		<h5>对象的引用</h5>
		<p style="text-indent:2em">位于Newtonsoft.Json命名空间；</p>
	<div>
	</div>
	<div>
		<h5>对象的创建</h5>
		<p style="text-indent:2em">
			是一个静态类，不能通过New关键字去构造一个对象；
		<p>				
	</div>	
	<div>
		<h5>对象的主要方法</h5>
		<li><b>SerializeObject</b>：序列化一个对象</li>
		可以用一个匿名类处理简单的数据结构：  
			`var o = new {Name = "windy",Age = 12,High = 175};`  
			`var strJson = JsonConvert.SerializeObject(o);`
		<li><b>DeserializeObject</b>：反序列化一个对象</li>
		可以用一个匿名类处理简单的数据结构：
		<ul>
			<li>提取局部信息</li>
			`var o = DeserializeObject(strJson) as JObject;`  
			`Console.Write(o.Name);`  
			`Console.Write(o.Age);`
			<li>提取完整信息</li>
			`var anonymous = new {Name =  String.Empty,Age = 0, High = 0} `  
			`var o DeserializeObject(strJson,anonymous)`  
			`Console.Write(o.Name);`  
			`Console.Write(o.Age);`
		</ul>
	</div>
</body>
</html>