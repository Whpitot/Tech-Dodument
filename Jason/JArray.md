<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>CSS概述</title>
</head>
<body>
    <div>
		<strong>
			模块：JArray<br/>
			时间：2017-07-17<br/>
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
		<p style="text-indent:2em">位于 Newtonsoft.Json.Linq命名空间；</p>
	<div>
	</div>
	<div>
		<h5>对象的创建</h5>
		<p style="text-indent:2em">
			通常是通过静态函数Parse创建一个新的对象；
			`String strJson={{"busiID":"12342","data":[{"Name":"windy","Age":12,"High":175},{"Name":"windy","Age":12,"High":175}]}}`
			`JObject jObject = JObject.Parse(strJson);`
			`JArray data = JArray.Parse(jObject["data"]); 单独提取一个对象`
			`Person person = Json.Convert.Deserialize<List<Person>>(data.Tostring());`
		<p>				
	</div>		
</body>
</html>