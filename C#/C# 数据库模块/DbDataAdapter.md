<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>C# 数据库连接模块</title>
</head>
<body>
    <div>
		<strong>
			模块：C# DbDataAdapter<br/>
			时间：2017-08-10<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>
	<div>
		<h3>DbProviderFactories</h3>
		<p>Aids implementation of the IDbDataAdapter interface.</p>
		<p>
			<strong>命名空间：</strong>System.Data.Common<br/>
			<strong>程序集：</strong>System.Data（位于 System.Data.dll）
		</p>
    </div>
	<div>
		<h4>语法</h4>
		<pre> public abstract class DbDataAdapter : DataAdapter, IDbDataAdapter, 
	IDataAdapter, ICloneable</pre>
	<div>
	<div>
		<h4>构造函数</h4>
		<div>
			<p>
				<strong>DbDataAdapter()</strong><br/>
				Initializes a new instance of a DataAdapter class.
			</p>
		</div>	
	</div>
	<div>
		<h4>属性</h4>
		<div>
			<p>
				<strong>SelectCommand</strong><br/>
					Gets or sets a command used to select records in the data source.
			</p>
		</div>	
	</div>
	<div>
		<h4>方法</h4>
		<div>
			<p>
				<strong>Fill(DataSet)</strong><br/>
				Adds or refreshes rows in the DataSet.
			</p>
			<pre>
ataSet dataSet = new DataSet();
dbDataAdapter.Fill(dataSet);
			</pre>
		</div>		
	<div>