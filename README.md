Tencent AlloyTeam
=================
One Team, One Dream! 多年以后，让我们创造一个奇迹！

By [Tencent AlloyTeam](http://www.AlloyTeam.com/)

## 我们的愿景

成为业界卓越的Web团队！


## 团队部分代码规范
虽然这些细节是小事，但是却体现了一个coder的专业程度。
更多详细情况请看：
alloyteam.github.com/DevelopmentCodes.doc


### 标准文件结构

	[mainfolder]
	 |--[js]		//js文件夹
	 |   |-- main.js
	 |--[style]		//所有样式相关的css和image
	 |   |-- [image]	//主要image文件夹
	 |   |    |-- img1.png
	 |   |    ...
	 |   |-- [styleNameA]	//皮肤A的文件夹
	 |   |    |-- [image]	//皮肤A的image
	 |   |    |-- styleNameA.css	//皮肤A的css文件
	 |   |    ...
	 |   |-- [styleNameB]	//皮肤B的文件夹
	 |   |-- [styleNameC]	//皮肤C的文件夹
	 |   |-- main.css	//主要css文件
 	 |-- index.html		//index文件
 	 |-- page1.html		//其他页面
 	 ...
	  
	  
ps：文件名全部英文小写，尽量不要加复数s，必要时可以使用下划线“_”。

	  
	  
### 标准html5代码

	<!DOCTYPE html>
	<html>
	<head>
		<meta charset="utf-8" />
		<meta name="author" content="Tencent.AlloyTeam.Jetyu" />
		<meta name="copyright" content="Tencent.AlloyTeam" />
		<title>Tencent AlloyTeam 标准文档</title>
		<link href="./style/main.css" rel="stylesheet" type="text/css" />
	</head>
	<body>
		<!-- 注释 -->
		<h1 id="title" class="title">Tencent AlloyTeam 标准文档</h1>
		<div>
			<h3>Title</h3>
			<p>
				标准文档
			</p>
		</div>

		<script type="text/javascript" src="./js/jx.min.js"></script>
		<script type="text/javascript">

		  var J = new Jx();

		</script>
	</body>
	</html>



### 标准javascript代码

	/**
	 * == Javascript eXtension 模块 =========================================================================
	 * Copyright (c) 2012 Tencent AlloyTeam, All rights reserved.
	 * http://www.AlloyTeam.com/
	 * Code licensed under the BSD License:
 	 * http://www.AlloyTeam.com/license.txt
	 * 
	 * @version 2.0
	 * @author	Kinvix(<a href="mailto:Kinvix@gmail.com">Kinvix@gmail.com</a>)
	 * @description 描述文字
	 * -------------------------------------------------------------- 2009.11.17 ----------------------------
	 */

	/**
	 * 注释
	 */
	Jx().$package("tencent.alloyteam", function(J){
		var packageContext = this,
			$D = J.dom,
			$E = J.event,
			$H = J.http;

		// 输出字符串：Hello world!
		J.out("Hello world!");

		// 输出this === tencent.alloyteam的判断结果
		J.out(this === tencent.alloyteam);
	});


### 标准css代码
	
	.copyright{
		margin:50px 0 0 0;
		height:50px;
		color:#999999;
		font-family:Tahoma;
		font-size: 12px;
		text-align:center;
	}

	.copyright a{
		color:#999999;
		text-decoration:none;
	}

	/* 注释 */
	.copyright a:hover,
	.copyright a:focus{
		outline:none;
		text-decoration:underline;
	}

### 标准版权声明代码

  	<div class="copyright">Copyright &copy; <script>document.write(new Date().getFullYear());</script> <a href="http://www.AlloyTeam.com/" target="_blank">Tencent AlloyTeam</a>. All Rights Reserved.</div>


### 标准访问统计代码

	<!--Tencent Analytics-->
	<script type="text/javascript" src="http://tajs.qq.com/stats?sId=8957212" charset="UTF-8"></script>
	<!--Google Analytics-->
	<script type="text/javascript">

	  var _gaq = _gaq || [];
	  _gaq.push(['_setAccount', 'UA-393149-9']);
	  _gaq.push(['_trackPageview']);

	  (function() {
	    var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
	    ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
	    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
	  })();

	</script>