<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>C# 数据库连接模块</title>
</head>
<body>
    <div>
		<strong>
			模块：C# DbConnection<br/>
			时间：2017-08-10<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>	
	<div>
		<h3>DbConnection</h3>
		<p>Represents a connection to a database.</p>
		<p>
			<strong>命名空间：</strong>System.Data.Common<br/>
			<strong>程序集：</strong>System.Data（位于 System.Data.dll）
		</p>
    </div>
	<div>
		<h4>语法</h4>
		<pre> public abstract class DbConnection : Component, IDbConnection,IDisposable</pre> 	
	</div>
	<div>
		<h4>属性</h4>
		<div>
			<p>
				<strong>ConnectionTimeout</strong><br/>
				Gets the time to wait while establishing a connection before terminating the attempt and generating an error.
			</p>
        </div>
		<div>
			<p>
				<strong>ConnectionString</strong><br/>
				Gets or sets the string used to open the connection.
			</p>
        </div>
	</div>
	<div>
		<h4>方法</h4>
		<div>
			<p>
				<strong>Open()</strong><br/>
				Opens a database connection with the settings specified by the ConnectionString.
			</p>
			<pre>dbConnection.Open();</pre>
		</div>
		<div>
			<p>
				<strong>CreateCommand()</strong><br/>
				Creates and returns a DbCommand object associated with the current connection.
			</p>
			<pre>DbCommand dbCommand = dbConnection.CreateCommand()</pre>
		</div>
		<div>
			<p>
				<strong>BeginTransaction()</strong><br/>
				Starts a database transaction.
			</p>
			<pre>DbTransaction dbTransaction = dbConnection.BeginTransaction();</pre>
		</div>
		<div>
			<p>
				<strong>Close()</strong><br/>
				Closes the connection to the database. This is the preferred method of closing any open connection.
			</p>
			<pre>dbConnection.Close();</pre>
		</div>
	</div>