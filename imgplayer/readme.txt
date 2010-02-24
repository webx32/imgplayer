jquery 图片播放器

作者：笑的自然
	我的博客：http://blog.csdn.net/xxd851116
	我的邮箱: xingxiudong@gmail.com

说明：
	1. 项目编码为GBK
	2. 目前播放模式支持 1:溶解，2:挂历模式，3:滑动(从左到右),4:滑动(从上到下),5:滑动(从下到上),6:滑动(从右到左)，善不支持随机模式
	3. 在IE6，IE8，FF下测试通过
	4. 支持任意数量图片，使用简单
	5. 考虑到图片占用空间较多，示例中图片来自网络，离线状态下需要自定义图片
	由于采用纯JavaScript实现，动画效果比较简单，目前善不支持随机播放模式，希望广大编程爱好者提出建议和不足。
	
参数：
	imgCSS		: 用户自定义图片样式
	transition	: 播放模式选项 1:溶解，2:挂历模式，3:滑动(从左到右),4:滑动(从上到下),5:滑动(从下到上),6:滑动(从右到左),23:随机
	width		: 播放器div容器的宽度
	height		: 播放器div容器的高度
	time		: 图片播放间隙时间,单位：毫秒
	duration	: 图片播放时间,单位：毫秒
	onStart		: 开始播放时执行的函数
	onStop		: 停止播放时执行的函数
	onShow		: 每页图片显示时执行的函数
	onHide		: 每页图片隐藏时执行的函数

使用示例:
	1. 容器代码
		<div id="imgContainer" style="margin-left:auto;margin-right:auto;margin-top:5px;display:none;">
			<a href="" target="_blank" title=""><img src="" title="" /></a>
			......
		</div>
	2. 导入jquery包（http://code.jquery.com/jquery-1.4.2.min.js）
		<script type="text/javascript" src="jquery-1.4.2.min.js"></script>
	3. 导入imgplayer包
		<script type="text/javascript" src="jquery.fn.imgplayer.min.js"></script>
	4. 绑定播放函数(参数说明详见上述)
		var player = $("#imgContainer").playImgs({
			imgCSS	: {'width' : '800px', 'height' : '600px'},
			width	: '800px',
			height: '600px',
			time	: '5000',
			transition : 1,
			duration : 2000
		}).start();
	

更新日志：
	v1.2(2010-02-24):
		1.修改了标题栏右侧冲出容器的bug
		2.添加了duration参数，可自定义图片动画效果时间
	
	v1.1(2009-09-23):
		1.修改了鼠标停留播放器和序号标签上图片继续播放的问题