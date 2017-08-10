<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>C# 数据库连接模块</title>
</head>
<body>
    <div>
		<strong>
			模块：C# DbCommand<br/>
			时间：2017-08-10<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>	
	<div>
		<h3>DbCommand</h3>
		<p>Represents an SQL statement or stored procedure to execute against a data source. Provides a base class for database-specific classes that represent commands.</p>
		<p>
			<strong>命名空间：</strong>System.Data.Common<br/>
			<strong>程序集：</strong>System.Data（位于 System.Data.dll）
		</p>
    </div>
	<div>
		<h4>语法</h4>
		<pre>public abstract class DbCommand : Component, IDbCommand, IDisposable</pre> 	
	</div>
    <div>
		<h4>属性</h4>
		<div>
			<p>
				<strong>CommandTimeout</strong><br/>
				Gets or sets the wait time before terminating the attempt to execute a command and generating an error.
			</p>
	    </div>
		<div>
			<p>
				<strong>Connection</strong><br/>
				Gets or sets the DbConnection used by this DbCommand.
			</p>
	    </div>
		<div>
			<p>
				<strong>CommandText</strong><br/>
				Gets or sets the text command to run against the data source.
			</p>
	    </div>
		<div>
			<p>
				<strong>CommandType</strong><br/>
				Indicates or specifies how the CommandText property is interpreted.
			</p>
	    </div>
		<div>
			<p>
				<strong>Parameters</strong><br/>
				Gets the collection of DbParameter objects.
			</p>
	    </div>
    </div>
	<div>
		<h4>方法</h4>
		<div>
			<p>
				<strong>CreateParameter()</strong><br/>
				Creates a new instance of a DbParameter object.
			</p>
			<pre>DbParameter dbParameter = dbCommand.CreateParameter();</pre>
		</div>
		<div>
			<p>
				<strong>ExecuteNonQuery()</strong><br/>
				Executes a SQL statement against a connection object.
			</p>
			<pre>int i = dbCommand.ExecuteNonQuery();</pre>
		</div>
		<div>
			<p>
				<strong>ExecuteScalar()</strong><br/>
				Executes the query and returns the first column of the first row in the result set returned by the query. All other columns and rows are ignored.
			</p>
			<pre>objec obj =dbCommand.ExecuteScalar(); </pre>
		</div>
		<div>
			<p>
				<strong>ExecuteReader()</strong><br/>
				Executes the CommandText against the Connection, and returns an DbDataReader.
			</p>
			<pre>DbDataReader dbDataReader = dbCommand.ExecuteReader();</pre>
		</div>
		<div>
			<p>
				<strong>ExecuteReader(CommandBehavior)</strong><br/>
				Executes the CommandText against the Connection, and returns an DbDataReader using one of the CommandBehavior values.<br/>
				例如：返回第一行记录
			</p>
			<pre>DbDataReader dbDataReader = dbCommand.ExecuteReader(CommandBehavior.SingelRow);</pre>
		</div>
	</div>