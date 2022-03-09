### <center>冬優ちゃんの个人网页</center>

<div align="center">
	<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width=340 height=86 src="//music.163.com/outchain/player?type=2&id=4943034&auto=0&height=66"></iframe>
	<img src="https://api.xhofe.top/ip/?line1=欢迎访问本站！&line2=fuibafuyu.top">
	<span id="jinrishici-sentence">正在加载今日诗词...</span>
	<script src="https://sdk.jinrishici.com/v2/browser/jinrishici.js" charset="utf-8"></script>
</div>

# <center>MC服务器</center>

## <center>游戏介绍</center>

游戏版本：Minecraft Bedrock Edition 1.18.10

游戏模式：生存

游戏难度：困难

作弊：否

在线验证：是

服务器地址：server.fuibafuyu.top:19132

## <center>游戏下载</center>

<a href="http://download.fuibafuyu.top/Program/Android/Minecraft/MCBE_1.18.10.04.apk">Android（解验证版）</a>

<a href="https://www.xbox.com/zh-cn/games/store/minecraft-for-windows/9nblggh2jhxj">Windows（Xbox）</a>

## <center>游戏视频（雾</center>

<div align="center">
	<iframe src="//player.bilibili.com/player.html?aid=80433022&bvid=BV1GJ411x7h7&cid=137649199&page=1&high_quality=1" allowfullscreen="allowfullscreen" width="100%" height="500" scrolling="no" frameborder="0" sandbox="allow-top-navigation allow-same-origin allow-forms allow-scripts"></iframe>
</div>

# <center>精简系统</center>

<a href="http://download.fuibafuyu.top/System/Windows/Lite/Win10-2004-YangLao-210919.iso">Windows 10 2004 养老版</a>

<a href="http://download.fuibafuyu.top/System/Windows/Lite/Win10-1803-Plus-ALPHA210208.iso">Windows 10 1803 精简增强版</a>

<a href="http://download.fuibafuyu.top/System/Windows/Lite/Win10-2009-Lite-ALPHA210320.iso">Windows 10 2009 精简版</a>

<a href="http://download.fuibafuyu.top/System/Windows/Lite/Win10-1703-Lite-ALPHA210206.iso">Windows 10 1703 精简版</a>

<a href="http://download.fuibafuyu.top/System/Windows/Lite/Win10-1809-Lite-ALPHA210311.iso">Windows 10 1809 精简版</a>

<a href="http://download.fuibafuyu.top/System/Windows/Lite/Win11-21H2-Lite-ALPHA211003.iso">Windows 11 21H2 精简版</a>

<a href="http://download.fuibafuyu.top/System/Windows/Lite/Win8.1-Plus-ALPHA210214.esd">Windows 8.1 精简增强版</a>

<a href="http://download.fuibafuyu.top/System/Windows/Lite/Win7-Lite-ALPHA210228.esd">Windows 7 精简版（ESD）</a>

<a href="http://download.fuibafuyu.top/System/Windows/Lite/Win7-Lite-ALPHA210228.iso">Windows 7 精简版（ISO）</a>

# <center>友情链接</center>

<a href="https://www.puresys.net/">Puresys</a>

<a href="https://firpe.cn/">FirPE</a>

<a href="https://easyig.site/">EasyIG</a>

<html>
	<head>
		<meta charset="UTF-8">
		<title></title>
		<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/font-awesome/css/font-awesome.min.css">
	</head>
	<body>
	</body>
	<script src="https://cdn.jsdelivr.net/gh/stevenjoezhang/live2d-widget/autoload.js"></script>
</html>

<script>

		(function(window,document,undefined){
			var hearts = [];
			window.requestAnimationFrame = (function(){
				return window.requestAnimationFrame ||
				window.webkitRequestAnimationFrame ||
				window.mozRequestAnimationFrame ||
				window.oRequestAnimationFrame ||
				window.msRequestAnimationFrame ||
				function (callback){
					setTimeout(callback,1000/60);
				}
			})();
			init();
			function init(){
				css(".heart{width: 10px;height: 10px;position: fixed;background: #f00;transform: rotate(45deg);-webkit-transform: rotate(45deg);-moz-transform: rotate(45deg);}.heart:after,.heart:before{content: '';width: inherit;height: inherit;background: inherit;border-radius: 50%;-webkit-border-radius: 50%;-moz-border-radius: 50%;position: absolute;}.heart:after{top: -5px;}.heart:before{left: -5px;}");
				attachEvent();
				gameloop();
			}
			function gameloop(){
				for(var i=0;i<hearts.length;i++){
					if(hearts[i].alpha <=0){
						document.body.removeChild(hearts[i].el);
						hearts.splice(i,1);
						continue;
					}
					hearts[i].y--;
					hearts[i].scale += 0.004;
					hearts[i].alpha -= 0.013;
					hearts[i].el.style.cssText = "left:"+hearts[i].x+"px;top:"+hearts[i].y+"px;opacity:"+hearts[i].alpha+";transform:scale("+hearts[i].scale+","+hearts[i].scale+") rotate(45deg);background:"+hearts[i].color;
				}
				requestAnimationFrame(gameloop);
			}
			function attachEvent(){
				var old = typeof window.onclick==="function" && window.onclick;
				window.onclick = function(event){
					old && old();
					createHeart(event);
				}
			}
			function createHeart(event){
				var d = document.createElement("div");
				d.className = "heart";
				hearts.push({
					el : d,
					x : event.clientX - 5,
					y : event.clientY - 5,
					scale : 1,
					alpha : 1,
					color : randomColor()
				});
				document.body.appendChild(d);
			}
			function css(css){
				var style = document.createElement("style");
				style.type="text/css";
				try{
					style.appendChild(document.createTextNode(css));
				}catch(ex){
					style.styleSheet.cssText = css;
				}
				document.getElementsByTagName('head')[0].appendChild(style);
			}
			function randomColor(){
				return "rgb("+(~~(Math.random()*255))+","+(~~(Math.random()*255))+","+(~~(Math.random()*255))+")";
			}
		})(window,document);
</script>
