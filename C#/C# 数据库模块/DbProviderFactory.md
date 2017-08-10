<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>C# 数据库连接模块</title>
</head>
<body>
    <div>
		<strong>
			模块：C# DbProviderFactory<br/>
			时间：2017-08-10<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>	
	<div>
		<h3>DbProviderFactories</h3>
		<p>Represents a set of methods for creating instances of a provider's implementation of the data source classes.</p>
		<p>
			<strong>命名空间：</strong>System.Data.Common<br/>
			<strong>程序集：</strong>System.Data（位于 System.Data.dll）
		</p>
    </div>
	<div>
		<h4>语法</h4>
		<pre> public abstract class DbProviderFactory;</pre>
	<div>
	<div>
	<h4>方法</h4>
	<div>
		<p>
			<strong>CreateConnection()</strong><br/>
			Returns a new instance of the provider's class that implements the DbConnection class.
		</p>
		<pre>DbConnection dbConnection = DbProviderFactory.CreateConnection()</pre>
	</div>