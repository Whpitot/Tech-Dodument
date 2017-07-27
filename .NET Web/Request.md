<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>CSS概述</title>
</head>
<body>
    <div>
		<strong>
			模块：.NET HttpWebRequest<br/>
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
		<p style="text-indent:2em">位于System.Net命名空间；</p>
	<div>
	</div>
	<div>
		<h5>对象的创建</h5>
		<p style="text-indent:2em">
			HttpWebRequset不是通过New一个对象来构造一个对象的。而是利用工厂机制(Factory Machanism)通过Create方法创建的；
		<p>		
		`HttpWebRequset request = HttpWebQuest.Create(Url) as HttpWebRequset`
	</div>
	<div>
		<h5>对象的主要属性</h5>
		<ul>
			<li><b>(String) Method</b>：数据的提交方式Post和Get；</li>
			`Request.Method ="post"`  
			`Request.Method ="get"`
			<li><b>(String)ContentType </b>：获取或设置传入请求的 MIME 内容类型	
				<ul>
					<li>application/json;</li>
				</ul>
			</li>
			`Request.ContentType ="application/json"`
			<li><b>ContentLength </b>：获取请求返回的内容的长度。</li>
			`Request.ContentLength =data.length`
			<li><b></b>：</li>
		</ul>
	</div>
	<div>
		<h5>对象的主要方法</h5>
		<li><b>(System.IO.Stream) GetRequestStream()</b>：获取一个流文件对象，然后将数据写入到流中</li>
		`System.IO.Stream requestStream = request.GetRequestStream()`
		`requestStream.Write(byteArray,0,byteArray.Length);`
		`requedtStream.Close();`
		<li><b>(WebResponse) GetResponse()</b>：返回来自 Internet 资源的响应。</li>
		`System.Net.HttpWebResponse response = request.GetResponse() as System.Net.HttpWebResponse;`
	</div>
</body>
</html>