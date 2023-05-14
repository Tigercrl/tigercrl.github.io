---
title: 404 Not Found
comments: false
permalink: /404.html
---
# <center>出现错误！(错误代码：404 Not Found)</center>

### <center id="404-text">你的JavaScript好像没开哦～</center>

### <center id="countdown">您未启用JavaScript，无法自动重定向至首页！</center>
### <center>您可以直接 **[点这里](/)** 返回首页</center>

<script>
  // 倒计时和重定向
  var redirectTime = new Date().getTime() + 5000;
  function count(){
  	if(new Date().getTime() >= redirectTime){
  		location.href = '/';
  	}else{
  		document.getElementById("countdown").innerHTML = "将在" + Math.ceil((redirectTime - new Date().getTime()) / 1000) + "秒后自动返回到首页";
  	}
  }
  count();
  window.onload = function () {
  	setInterval("count()", 100);
  }
  // 404提示
  var texts = [
	"你要找的页面被人揉巴揉巴扔了..",
	"你要找的页面现已退役..",
	"Sssss.. 什么声音? Sss.. 啊.. BOOM!",
	"你要找的页面似乎没能和你达成共识..",
	"你要找的页面带着狗去捡垃圾了..",
	"我想这个页面走了一些弯路..",
	"你要找的页面似乎不能和你同台竞技..",
	"你要找的页面回家过节了..",
	"你要找的页面坐着矿车逃走了..",
	"你要找的页面被人丢进了打粉机..",
	"你要找的页面爆炸了!!",
	"我们对此页面无法显示表示强烈谴责..",
	"你要找的页面被恶魂烧焦了..",
	"你要找的页面被铁傀儡一巴掌拍飞了!",
	"你要找的页面被外星人抓走了..",
	"你或许可以为此页面造一个“刷页笼”..",
	"你要找的页面掉!漆!了!..",
	"你要找的页面似乎坠入了虚空..",
	"你要找的页面去打麻将了..",
	"你要找的页面上面坐着一只豹猫..",
	"你要找的页面被雨淋湿了..",
	"你要找的页面正处于量子叠加态..",
	"你要找的页面被吃掉了!",
	"你要找的页面被史莱姆一屁股坐扁了!",
	"从前有座山，山上有座庙，庙里有个页面，现在找不到！"
];
document.getElementById('404-text').innerHTML = texts[parseInt(Math.random()*(texts.length)+1,10)];
</script>