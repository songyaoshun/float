float异常汇总
==================================
### 1.背景不能显示，边框不能撑开。(直接上代码)
`未浮动代码`
```html
<!DOCTYPE html>
<html>
<head>
	<title>css float</title>
</head>
<body>
	<div class="" style="background: green;border: 1px solid">
		<div class="" style="background: red;width: 100px;height: 100px;">
		</div>
	</div>
</body>
</html>
```
`效果如下：`  
![未浮动效果](https://github.com/songyaoshun/float/blob/master/1st.jpg)  

`下面添加浮动之后父级将不会被展开`
```html
<!DOCTYPE html>
<html>
<head>
	<title>css float</title>
</head>
<body>
	<div class="" style="background: green;border: 1px solid">
		<div class="" style="background: red;width: 100px;height: 100px;float: left;">
		</div>
	</div>
</body>
</html>
```
`效果如下：`  
![浮动效果](https://github.com/songyaoshun/float/blob/master/2nd.jpg)  

### 2.添加浮动后，父级的padding不能正确显示,margin 效果尚可
`未浮动代码`  
```html
<!DOCTYPE html>
<html>
<head>
	<title>css float</title>
</head>
<body>
	<div class="" style="background: pink;width: 300px;height: 100px;"></div>
	<div class="" style="background: green;border: 1px solid;margin: 50px;padding: 10px">
		<div class="" style="background: red;width: 100px;height: 100px;">
		</div>
	</div>
	<div class="" style="background: pink;width: 300px;height: 100px;margin-top: 10px"></div>
</body>
</html>
```
`效果如下：`
![未浮动效果](https://github.com/songyaoshun/float/blob/master/3rd.jpg)  
`未浮动代码`  
```html
<!DOCTYPE html>
<html>
<head>
	<title>css float</title>
</head>
<body>
	<div class="" style="background: pink;width: 300px;height: 100px;"></div>
	<div class="" style="background: green;border: 1px solid;margin: 50px;padding: 10px">
		<div class="" style="background: red;width: 100px;height: 100px;float: left;">
		</div>
	</div>
	<div class="" style="background: pink;width: 300px;height: 100px;margin-top: 10px"></div>
</body>
</html>
```
`效果如下：`
![未浮动效果](https://github.com/songyaoshun/float/blob/master/4th.jpg)