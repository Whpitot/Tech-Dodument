<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>C# 数据库连接模块</title>
</head>
<body>
    <div>
		<strong>
			模块：C# DataTable<br/>
			时间：2017-08-10<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>	
	<div>
		<h3>DataTable</h3>
		<p>Represents one table of in-memory data.</p>
		<p>
			<strong>命名空间：</strong>System.Data<br/>
			<strong>程序集：</strong>System.Data（位于 System.Data.dll）
		</p>
    </div>
	<div>
		<h4>语法</h4>
		<pre>[SerializableAttribute]
public class DataTable : MarshalByValueComponent, IListSource, 
	ISupportInitializeNotification, ISupportInitialize, ISerializable, 
	IXmlSerializable
       </pre> 	
	</div>
	<div>
		<h4>构造函数</h4>
		<div>
			<p>
				<strong>DataTable()</strong><br/>
				Initializes a new instance of the DataTable class with no arguments.
			</p>
			<pre>DataTable dataTable = new DataTable()</pre>
		</div>	
		<div>
			<p>
				<strong>DataTable(String)</strong><br/>
				Initializes a new instance of the DataTable class with the specified table name.
			</p>
			<pre>DataTable dataTable = new DataTable("Windy")</pre>
		</div>	
	</div>
 	<div>
		<h4>属性</h4>
		<div>
			<p>
				<strong>Columns</strong><br/>
				Gets the collection of columns that belong to this table.
			</p>
	    </div>
		<div>
			<p>
				<strong>Rows</strong><br/>
				Gets the collection of rows that belong to this table.
			</p>
	    </div>
		<div>
			<p>
				<strong>PrimaryKey</strong><br/>
				Gets or sets an array of columns that function as primary keys for the data table.
			</p>
	    </div>
		<div>
			<p>
				<strong>DefaultView</strong><br/>
				Indicates or specifies how the CommandText property is interpreted.
			</p>
	    </div>
		<div>
			<p>
				<strong>Parameters</strong><br/>
				Gets a customized view of the table that may include a filtered view, or a cursor position.
			</p>
	    </div>
    </div>
	<div>
		<h4>方法</h4>
		<div>
			<p>
				<strong>Clear()</strong><br/>
				Clears the DataTable of all data.
			</p>
			<pre>dataTable.Clear()</pre>
		</div>
		<div>
			<p>
				<strong>Clone()</strong><br/>
				Clones the structure of the DataTable, including all DataTable schemas and constraints.
			</p>
			<pre>DataTable table = dataTable.Clone() </pre>
		</div>
		<div>
			<p>
				<strong>ImportRow(DataRow)</strong><br/>
				Copies a DataRow into a DataTable, preserving any property settings, as well as original and current values.
			</p>
			<pre>dataTable.ImportRow(dataRow);</pre>
		</div>
		<div>
			<p>
				<strong>NewRow()</strong><br/>
				Creates a new DataRow with the same schema as the table.
			</p>
			<pre>dataRow = dataTable.NewRow();</pre>
		</div>
		<div>
			<p>
				<strong>Select(String)</strong><br/>
				Gets an array of all DataRow objects that match the filter criteria.
			</p>
			<pre>DataRow[] dataRow = dataTable.Select("Name = 'windy'");</pre>
		</div>
	</div>
	<div>
		<h4>事件</h4>
		<div>
			<p>
				<strong>ColumnChanged</strong><br/>
				Occurs after a value has been changed for the specified DataColumn in a DataRow.
			</p>
			<pre>
private static void Column_Changed(object sender, DataColumnChangeEventArgs e )
{
    if(e.ColumnName == “windy”)
	{
		Console.WriteLine("Hello Wrold")；
	}
}
		</pre>
		</div>
	</div>