<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
    <title>SqlServer 数据库模块</title>
</head>
<body>
    <div>
		<strong>
			模块：SqlServer Table<br/>
			时间：2017-08-11<br/>
			编写人：小帅<br/>
			版本：V1.0						
		</strong>
	</div>	
    <hr/>	
	<div>
		<h3>Table</h3>
		<p>
			Tables are database objects that contain all the data in a database.<br/>
			Each row represents a unique record, and each column represents a field in the record.
		</p>
    </div>
	<div>
		<h4>表操作</h4>
		<div>
			<p>
				<strong>Create Tables</strong><br/>
			</p>
			<pre>
Create Table Student (
	_ID varchar(50) primarykey,
	Name varchar(50) not null,
	Age int null,
	Sex bit null
);         </pre>
		</div>
	</div>
		<div>

			<p>
				<strong>Create Tables</strong><br/>
			</p>
			<pre>
Create Table Student (
	_ID varchar(50) primarykey,
	Name varchar(50) not null,
	Age int null,
	Sex bit null
);         </pre>
	</div>
