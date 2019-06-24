![markdown](https://camo.githubusercontent.com/728ce9f78c3139e76fa69925ad7cc502e32795d2/68747470733a2f2f7675656a732e6f72672f696d616765732f6c6f676f2e706e67 "vue")

## Vue的指令学习
### v-show
	v-show根据条件来判断显示标签，功能与v-if类似。
```html
<html>
    	<head>
		<meta charset="utf-8">
		<title>v-show指令学习</title>
		<script src="https://cdn.bootcss.com/vue/2.2.2/vue.min.js"></script>
		</head>
		<body>
		<div id="app">
		    <h1 v-show="ok">Hello!</h1>  //条件为TRUE，输出
		    <h1 v-show="error">false!</h1>  //条件为false，不输出
		    <h1 v-show="10>5">10大于5，输出!</h1>   //条件为TRUE，输出
		    <h1 v-show="2>10">不大于10，不输出!</h1>   //条件为false，不输出
		</div>
		    
		<script>
		new Vue({
		  el: '#app',
		  data: {
		    ok: true,
		    error: false
		  }
		})
		</script>
	</body>
	</html>
```
