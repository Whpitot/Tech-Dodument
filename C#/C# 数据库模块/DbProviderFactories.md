<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>C# 数据库连接模块</title>
</head>
<body>
    <div>
		<strong>
			模块：C# DbProviderFactories<br/>
			时间：2017-08-10<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>
	<div>
		<h3>DbProviderFactories</h3>
		<p>Represents a set of static methods for creating one or more instances of DbProviderFactory classes.</p>
		<p>
			<strong>命名空间：</strong>System.Data.Common<br/>
			<strong>程序集：</strong>System.Data（位于 System.Data.dll）
		</p>
    </div>
	<div>
		<h4>语法</h4>
		<pre> public static class DbProviderFactories;</pre>
	<div>
	<div>
		<h4>方法</h4>
		<div>
			<p>
				<strong>GetFactory(String)</strong><br/>
				Returns an instance of a DbProviderFactory.
			</p>
			<pre>DbProviderFactory DbProviderFactory = DbProviderFactories.GetFactory(InvariantName);</pre>
		</div>
		<div>
			<p>
				<strong>GetFactoryClasses()</strong><br/>
				Returns a DataTable that contains information about all installed providers that implement DbProviderFactory.
			</p>
			<pre> DataTable dataTable = DbProviderFactories.GetFactoryClasses();</pre>
			<table>
				<th>Name</th>
				<th>Desctiption</th>
				<th>InvariantName</th>
				<th>AssemblyQualifiedName</th>
				<tr>
					<td>OracleClient Data Provider</td>
					<td>.Net Framework Data Provider for Oracle</td>
					<td>System.Data.OracleClient</td>
					<td>System.Data.OracleClient.OracleClientFactory, System.Data.OracleClient, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089</td>
				<tr>	
				<tr>
					<td>SqlClient Data Provider</td>
					<td>.Net Framework Data Provider for SqlServer</td>
					<td>System.Data.SqlClient</td>
					<td>System.Data.SqlClient.SqlClientFactory, System.Data, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089</td>
				<tr>
			</table>
		</div>
	<div>