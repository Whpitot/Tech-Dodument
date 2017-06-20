<!doctype html>
<html>
	<header>
		<title>Html中的表单<title>
		<meta charset="utf-8"></meta>
	</header>
	<body>	
		<div>
			<strong>
				模块：Html5中的表单</br>
				时间：2017-06-20</br>
				编写人：小帅</br>
				版本：V1.0
			</strong>
		</div>
		<h2>Html5中的表格</h2>
		<h6>表单From</h6>
		<ul>
			<li>说明：用来收集网页上浏览者输入的相关信息</li>
			<li>基本属性：Method="post|get"&nbsp;&nbsp; Action="url" </li>
		</ul>	
		<hr>
		<h6>表单基本元素</h6>
		<ul>	
			<li><b>text:</b> name="" size="" maxlength="" value="" </li>
            <li><b>textarea:</b> name="" cols="" rows="" wrap=""</li>
			<li><b>password:</b> name="" sieze="" maxlength=""</li>
			<li><b>radio：</b> name=""【一组需要为同一名字】 checked="checked"</li>
			<li><b>checkbox:</b> name="" 【一组需要为同一名字】 </li>
			<li><b>select:</b> name="" size="" selected="" </li>
			<li><b>button:</b> name="" value="" onclick=""</li>
			<li><b>submit:</b> name="" value=""</li>
			<li><b>reset:</b>name="" value=""</li>
		</ul>
		<h6>表单高级元素</h6>
		<ul>
			<li><b>file:</b>name="" </li>
			<li><b>url:</b>name=""</li>
			<li><b>email:</b>name=""</li>
			<li><b>date:</b>name=""</li>
			<li><b>times:</b>name=""</li>
			<li><b>number:</b>name=""</li>
			<li><b>range:</b>name="" max="" min=""</li>
			<li><b>required:</b>required="required"</li>
		</ul>
		<hr>	
		<div>
			<h2>系统登录</h2>			
		</div>
		<div>
			<form method="" action="" >
				<label>邮&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;箱：</label>	
				<input type="email" required="required" name="uEmail" placeholder="请输入邮箱"></input></br>		
				<label>昵&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;称：<label>
				<input type="text" required="required" name="uName" placeholder="请输入昵称"></input></br>
				<label>密&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;码：<label>
				<input type="password" required="required" name="uPwd" placeholder="请输入密码"></input></br>
				<label>性&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;别：<label>				
				<input type="radio" name="sex" checked="checked">男</input>
				<input type="radio" name="sex">女</input>
				<input type="radio" name="sex">保密</input></br>		
				<lable>个性签名：<lable></br>
				<textarea cols="26" rows="3"></textarea></br>
				<input type="submit"  value="提交">
				<input type="reset" value="重设">
			</form>
		</div>
	</dody>
</html>