<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>C# 数据库连接模块</title>
</head>
<body>
    <div>
		<strong>
			模块：C# DbDataReader<br/>
			时间：2017-08-10<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>	
	<div>
		<h3>DbProviderFactories</h3>
		<p>Reads a forward-only stream of rows from a data source.</p>
		<p>
			<strong>命名空间：</strong>System.Data.Common<br/>
			<strong>程序集：</strong>System.Data（位于 System.Data.dll）
		</p>
    </div>
	<div>
		<h4>语法</h4>
		<pre>public abstract class DbDataReader : MarshalByRefObject, IDataReader, 
	IDisposable, IDataRecord, IEnumerable</pre>
	</div>
	<div>
		<h4>属性</h4>
		<p>
			<strong>FieldCount<br/></stong>
			Gets the number of columns in the current row.
		</p>
	</div>
	<div>
		<h4>方法</h4>
		<div>
			<p>
				<strong>Read()</strong><br/>
				Advances the reader to the next record in a result set.
			</p>
			<pre>if( dbDataReader.Read() )
	{
		string Name = dbDataReader["Name"];
	}
	</pre>
		</div>
		<div>
			<p>
				<strong>GetName(Int32)</strong><br/>
				Gets the name of the column, given the zero-based column ordinal.
			</p>
			<pre>dataTable.Columns.Add(dbDataReader.GetName(i));</pre>
		</div>
		<div>
			<p>
				<strong>GetFieldType(Int32)</strong><br/>
				Gets the data type of the specified column.
			</p>
			<pre>DataColumn dataColumn = new DataColumn(dbDataReader.GetName(i),GetFieldType(Int32))</pre>
		</div>
		<div>
			<p>
				<strong>GetValue(Int32)</strong><br/>
				Gets the value of the specified column as an instance of Object.
			</p>
			<pre>object obj = GetValue(Int32)</pre>
		</div>		
		<div>
			<p>
				<strong>GetValue(Int32)</strong><br/>
				Gets the value of the specified column as an instance of Object.
			</p>
			<pre>
object[] values = new object[dbDataReader.FieldCount];
dbDataReader.GetValues(values);
dataTable.Rows.Add(values);
			</pre>
		</div>	
	</div>