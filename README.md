

|      属性     |     含义      |      初始值     |    重要性      |
| ------------- |:-------------:| ------------- |:-------------:|
| name     |菜单的名称 |  无     |必须 | 
| onClick     |点击执行的函数 |  无     |必须 | 



##代码展示
```javascript
<body>
<div class="container">
	<h4 id="demo1">Demo 1</h4>
	<p>在这个例子中，在下面的矩形区域内右键点击就可以打开上下文菜单。</p>

	<div class="row collapsibleContainer">
		<div class="col-md-6">
			<div id="demo1Box" class="text-center" style="height: 300px; border:1px solid #ddd">
				<span style="line-height: 300px">在这个区域内的任何位置点击右键</span>
			</div>
		</div>
	</div>
</div>

<script>
var menu = new BootstrapMenu('#demo1Box', {
  actions: [{
	name: 'jQuery',
	onClick: function() {
	  alert("jQuery");
	}
  }, {
	name: 'HTML5',
	onClick: function() {
	  alert("HTML5");
	}
  }, {
	name: 'tricks',
	onClick: function() {
	  alert("tricks");
	}
  }]
});
</script>
</body>
```
##效果演示：
![mahua](http://myweb-10017157.file.myqcloud.com/gif/131171306754898987.gif)
