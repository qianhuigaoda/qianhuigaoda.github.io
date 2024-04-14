<!DOCTYPE html>
<html lang="en">
<head>
	<style>
	body {
	  background-color: #f2f2f2; /* 灰色的RRGGBB十六进制代码 */
	}
	</style>
	<meta charset="UTF-8">
	<title>主页</title>
<style>
  /* 样式定义 */
  body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
    }
	.header {
    position: fixed; /* 固定位置 */
		top: 0; /* 固定在顶部 */
		width: 100%; /* 宽度占满整个页面 */
		left: 0; /* 固定在左侧 */
		display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px;
    background-color: #f8f9fa;
		z-index: 999; /* 确保在其他内容之上 */
  }

  .logo-image {
    width: 400px; /* 根据需要调整图片宽度 */
    height: 65px; /* 保持图片比例 */
  }

  .header-right {
    display: flex;
    align-items: center;
  }

  .icon {
    width: 30px; /* 图标宽度 */
    height: 30px; /* 图标高度 */
    margin-right: 5px; /* 图标与文字之间的间距 */
  }

  .link {
    color: #007bff;
    text-decoration: none;
		margin-right: 25px;
  }
	
</style>
</head>
<body>
  <!-- HTML结构 -->
  <header class="header">
    <img class="logo-image" src="https://pic.imgdb.cn/item/661c4dfb68eb935713bd5216.png" alt="Logo"> <!-- 替换为你的图片路径 -->
    <div class="header-right">
      <img class="icon" src="https://pic.imgdb.cn/item/661c4ee768eb935713bdf652.png" alt="Icon"> <!-- 替换为你的图标路径 -->
      <a class="link" href="https://htmlpreview.github.io/?https://github.com/qianhuigaoda/qianhuigaoda.github.io/blob/master/paper.html">论文板块</a> <!-- 替换为你的链接文字和URL -->
			<img class="icon" src="https://pic.imgdb.cn/item/661c4ede68eb935713bdeee4.png" alt="Icon"> <!-- 替换为你的图标路径 -->
			<a class="link" href="https://htmlpreview.github.io/?https://github.com/qianhuigaoda/qianhuigaoda.github.io/blob/master/author.html">作者板块</a> <!-- 替换为你的链接文字和URL -->
			<img class="icon" src="https://pic.imgdb.cn/item/661c4edf68eb935713bdf038.png" alt="Icon"> <!-- 替换为你的图标路径 -->
			<a class="link" href="https://htmlpreview.github.io/?https://github.com/qianhuigaoda/qianhuigaoda.github.io/blob/master/touga.html">投稿板块</a> <!-- 替换为你的链接文字和URL -->
    </div>
  </header>
<main>
	<style>
		/* 样式定义 */
		.main-content {
		    margin-top: 200px; /* 这里设置间距大小 */
		    padding: 20px;
		    max-width: 1200px;
		    margin: 0 auto; /* 水平居中 */
		  }
		.image-container {
			position: relative;
	    height: 350px;
			width: 800px;
	    max-width: 1200px;
	    margin: 0 auto;
	  }
	
	  .image-container img {
	    height: 400px;
			width: 100%;
	    display: block;
			margin-top: 100px;
	  }
	
	  .circle-container {
	    display: flex;
	    justify-content: center;
	    margin-top: 65px;
	  }
	
	  .circle {
	    width: 30px;
	    height: 30px;
	    border-radius: 100%;
	    background-color: #ddd;
	    margin: 0 5px;
	    cursor: pointer;
	  }
	
	  .circle.active.active {
	    background-color: #007bff;
	  }
	</style>
	<main class="main-content">
	<div class="image-container">
	  <img id="image" src="https://pic.imgdb.cn/item/661c4dfe68eb935713bd54af.png" alt="Image 1">
	</div>
	
	<div class="circle-container">
	  <div class="circle" data-image="https://pic.imgdb.cn/item/661c4dfe68eb935713bd54af.png" onclick="changeImage(this)"></div>
		<div class="circle" data-image="https://pic.imgdb.cn/item/661c4df468eb935713bd4d70.png" onclick="changeImage(this)"></div>
	  <div class="circle" data-image="https://pic.imgdb.cn/item/661c4e6b68eb935713bda185.png" onclick="changeImage(this)"></div>
	  <div class="circle" data-image="https://pic.imgdb.cn/item/661c4e1468eb935713bd6374.png" onclick="changeImage(this)"></div>
		<div class="circle" data-image="https://pic.imgdb.cn/item/6610113468eb93571342835d.png" onclick="changeImage(this)"></div>
	</div>
	
	<script>
	  // JavaScript函数来切换图片
	  function changeImage(circle) {
	    // 移除之前所有圆圈的激活状态
	    var circles = document.querySelectorAll('.circle');
	    circles.forEach(function(circle) {
	      circle.classList.remove('active');
	    });
	
	    // 激活被点击的圆圈
	    circle.classList.add('active');
	
	    // 获取图片元素
	    var imageElement = document.getElementById('image');
	
	    // 切换图片源
	    imageElement.src = circle.getAttribute('data-image');
	  }
	</script>
</main>
</div>
<style>
	.icon {
	  width: 30px; /* 图标宽度 */
	  height: 30px; /* 图标高度 */
	  margin-right: 5px; /* 图标与文字之间的间距 */
	}
</style>
<div class="header-right">
      <img class="icon" src="https://pic.imgdb.cn/item/661c4eff68eb935713be085d.png" alt="Icon"> <!-- 替换为你的图标路径 -->
      <h2><p>东辉科学报部分精选论文</p></h2> <!-- 替换为你的链接文字和URL -->
</div>

<title>论文区域</title>
<style>
	.container {
    display: flex; /* Use Flexbox layout */
  }
  .boder {
    flex: 0 0 25%; /* Each box takes up a quarter of the width */
    border: 1px solid #000; /* Border for visualization */
    box-sizing: border-box; /* Ensure border is included in box size */
    padding: 10px; /* Optional padding */
    min-width: 400px; /* Minimum width of the box */
    min-height: 600px; /* Minimum height of the box */
    text-align: center; /* Center the text inside the box */
		margin: 0 auto ;
  }
	.boder img {
	    width: 350px; /* 设置图片的宽度 */
	    height: 320px; /* 设置图片的高度 */
	    display: block; /* 使图片在边框内居中 */
	    margin: 0 auto;
	  }
	.boder a {
					text-decoration: none;
					color: blue;
			    padding: 5px 10px;
					text-align: left; /* 设置文字居中 */
					display: inline-block;
			  }
</style>
</head>
<body>
<div class="container">
  <div class="boder">
		<h2 align="center"><P>不同水位下水压和密度的差异与重力分布趋势的关联</P>
		    <p>作者：王东辉几何</p></h2>
      <img src="https://pic.imgdb.cn/item/6610113d68eb935713429b39.png" alt="Image 1">
    </a>
    <h3><a href="https://htmlpreview.github.io/?https://github.com/qianhuigaoda/qianhuigaoda.github.io/blob/master/paper/1.html">此项研究通过调查不同水位和高度下水压和密度的差异规律。归纳出一个适用于地球重力空间的物理定律。即：“在地球重力空间的一个容器内，水体的质点越接近重力加速度大的区域，其密度和压强越大，反之越小”。然后...</a></h3>
  </div>
  <div class="boder"><h2 align="center"><P>黑魔法咏唱字节序列的分析与不同组合效果的差异</P>
		    <p>作者：王东辉魔法</p></h2>
      <img src="https://pic.imgdb.cn/item/6610113968eb935713429001.png" alt="Image 2">
    </a>
    <h3><a href="https://htmlpreview.github.io/?https://github.com/qianhuigaoda/qianhuigaoda.github.io/blob/master/paper/2.html">黑魔法作为强大的力量，在魔法学院的教学中拥有重要的地位。黑魔法的咏唱过程中使用的特定字节序列，对于施法者而言具有重要意义。本文通过深入分析黑魔法咏唱字节序列的特征，并通过实验研究不同组合方式对黑魔法效果的影响来作为判断依据。旨在探讨黑魔法咏唱字节序列的分析与不同组合方式之间的差异。通过这些研究结果，我们...</a></h3>
  </div>
  <div class="boder"><h2 align="center"><P>东辉宇宙一新种记述</P>
		    <p>作者：王东辉几何</p></h2>
      <img src="https://pic.imgdb.cn/item/6610113068eb9357134278e0.png" alt="Image 3">
    </a>
    <h3><a href="https://htmlpreview.github.io/?https://github.com/qianhuigaoda/qianhuigaoda.github.io/blob/master/paper/3.html">本文研究了东辉宇宙中新的学科：王东辉几何 Geometria	wangdonghuae。通过对该物种的行为、形态以及分布特征的观察和实验，揭示了其隶属于民科和几何属的分类学归属。研究发现，王东辉几何具有形态变化多端的特点，在民科的各个领域中能够形成不同的摸样和模式，尽管如此总能通过其特有的...</a></h3>
  </div>
  <div class="boder"><h2 align="center"><P>元素反应与新能源的应用</P>
        <p>作者：王西辉原神</p></h2>
      <img src="https://pic.imgdb.cn/item/66144e3768eb935713fcab83.png" alt="Image 4">
    </a>
    <h3><a href="https://htmlpreview.github.io/?https://github.com/qianhuigaoda/qianhuigaoda.github.io/blob/master/paper/11.html">随着全球能源需求的不断增长，元素反应的开发与应用成为当前研究的热点。元素反应作为新能源技术的基础，其研究对于推动新能源领域的发展具有重要意义。本文首先分析了元素反应的基本原理及其在新能源领域的应用现状，随后重点探讨了新能源中元素反应的两大类，分别是“增幅反应”和“剧变反应”的应用及其优势，最后对新能源的发展趋势进行了展望。</a></h3>
  </div>
</div>
<style>
	.icon {
	  width: 30px; /* 图标宽度 */
	  height: 30px; /* 图标高度 */
	  margin-right: 5px; /* 图标与文字之间的间距 */
	}
</style>
<div class="header-right">
      <img class="icon" src="https://pic.imgdb.cn/item/661c4eff68eb935713be085d.png" alt="Icon"> <!-- 替换为你的图标路径 -->
      <h2><p>东辉科学报部分作者展示</p></h2> <!-- 替换为你的链接文字和URL -->
</div>
<title>作者区域</title>
<style>
	.box-container {
    display: flex; /* Use Flexbox layout */
  }
  .box {
    flex: 0 0 25%; /* Each box takes up a quarter of the width */
    border: 1px solid #000; /* Border for visualization */
    box-sizing: border-box; /* Ensure border is included in box size */
    padding: 10px; /* Optional padding */
    min-width: 400px; /* Minimum width of the box */
    min-height: 600px; /* Minimum height of the box */
    text-align: center; /* Center the text inside the box */
		margin: 0 auto ;
  }
	.box img {
	    width: 350px; /* 设置图片的宽度 */
	    height: 500px; /* 设置图片的高度 */
	    display: block; /* 使图片在边框内居中 */
	    margin: 0 auto;
	  }
	.box text {
					text-decoration: none;
			    padding: 5px 10px;
					text-align: left; /* 设置文字居中 */
					display: inline-block;
			  }
</style>
<div class="box-container">
  <div class="box">
    <h3><p align="center">王东辉魔法</p></h3>
		<img src="https://pic.imgdb.cn/item/661005c768eb9357132d99a5.jpg" alt="图片">
    <h3><p align="left">Exploring the mysteries of magic is also exploring the essence of this universe</p></h3>
		<h3><p align="left">探索魔法的奥秘，也是在探索这个宇宙的本质</p></h3>
  </div>

	  <div class="box">
	    <h3><p align="center">王东辉高达</p></h3>
	  	<img src="https://pic.imgdb.cn/item/661005c668eb9357132d9931.png" alt="图片">
	    <h3><p align="left">Truth is only within the range of my cannon</p></h3>
	  	<h3><p align="left">真理只在我的大炮射程之内</p></h3>
	  </div>
			
			  <div class="box">
			    <h3><p align="center">王东辉佛学</p></h3>
					<img src="https://pic.imgdb.cn/item/661450bd68eb935713ffd5a8.png" alt="图片">
			    <h3><p align="left">Learn the Dawei Tianlong and Dafa spells from me and you'll be able to see and break the pirate Wang Donghui's gold coin space transfer magic</p></h3>
					<h3><p align="left">跟我学大威天龙和大罗法咒就能参悟和破解王东辉海盗的金币空间转移魔法</p></h3>
			  </div>
				
				  <div class="box">
				    <h3><p align="center">王东辉足球</p></h3>
						<img src="https://pic.imgdb.cn/item/661005d968eb9357132d9f29.jpg" alt="图片">
				    <h3><p align="left">No matter how much effort, no matter how much sea cucumber is eaten, or how devout a prayer is, it cannot be saved. I feel powerless</p></h3>
						<h3><p align="left">即使做再多的努力、吃再多的海参、或者再虔诚的祈祷都不能挽救它，我觉得无能为力</p></h3>
				  </div>
					
</div>
<footer>
<title>Image Row</title>
<style>
  .box-boder-container {
    display: flex; /* Use Flexbox layout */
  }
  .box-boder {
    flex: 0 0 25%; /* Each box takes up a quarter of the width */
    border: auto; /* Border for visualization */
    box-sizing: border-box; /* Ensure border is included in box size */
    padding: 5px; /* Optional padding */
    min-width: 800px; /* Minimum width of the box */
    min-height: 200px; /* Minimum height of the box */
		margin: 10px;
  }
	.box-boder img {
	    width: 800px; /* 设置图片的宽度 */
	    height: 400px; /* 设置图片的高度 */
	    display: block; /* 使图片在边框内居中 */
			margin: 15px auto;
			margin-left: 25px;
			margin-right: 25px;
	}
</style>
<div class="box-boder-container">
	<div class="box-boder">
  <img src="https://pic.imgdb.cn/item/661c4d9268eb935713bd0cc5.png" alt="Footer Image" class="boder-image">
</div>

  <div class="box-boder">
	<img src="https://pic.imgdb.cn/item/661c4e2668eb935713bd6e04.png" alt="Footer Image" class="boder-image">
</div>
</div>
<h3><p align="center">&copy; Donghui Science Daily 2023</p></h3>
</footer>
</html>

</html>
