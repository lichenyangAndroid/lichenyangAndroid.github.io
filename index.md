<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>这是一个demo</title>
	<style>
		*{
			margin:0;
			padding:0;
		}
		body,html{
            height:100%;
            background:#000;
		}
		ul,ol,li{
			list-style:none;
		}
		body{
			height:100%;
			background:url(img/bg.jpg) no-repeat;
			background-size:100% 100%;
		}
		section{
			box-shadow: 0 2px 100px #fff
		}
		section:first-of-type{
			width:500px;
			height:500px;
			position:fixed;
			left:0;
			right:0;
			top:0;
			bottom:0;
			margin:auto;
			border-radius: 100%;
			transform:rotateX(70deg) rotateY(-20deg);
			transform-style: preserve-3d;	
			animation: move1 15s linear infinite;
			box-shadow:none;
		}
		section:first-of-type ul{
			position:absolute;
			width:300px;
			height:300px;
			left:50%;
			top:50%;
			margin:-150px 0 0 -150px;
			border-radius: 100%;
			transform-style: preserve-3d;
		}
		section:first-of-type ul li{
			width:100%;
			height:100%;
			border:1px solid orange;
			position:absolute;
			border-radius: 100%;
			box-shadow: 0 2px 20px orange;
		}

		ul li:first-child{
			transform:rotateY(20deg);
		}
		ul li:nth-child(2){
			transform:rotateY(40deg);
		}
		ul li:nth-child(3){
			transform:rotateY(60deg);
		}
		ul li:nth-child(4){
			transform:rotateY(80deg);
		}
		ul li:nth-child(5){
			transform:rotateY(100deg);
		}
		ul li:nth-child(6){
			transform:rotateY(120deg);
		}
		ul li:nth-child(7){
			transform:rotateY(140deg);
		}
		ul li:nth-child(8){
			transform:rotateY(160deg);
		}
		ul li:nth-child(9){
			transform:rotateX(20deg);
		}
		ul li:nth-child(10){
			transform:rotateX(40deg);
		}
		ul li:nth-child(11){
			transform:rotateX(60deg);
		}
		ul li:nth-child(12){
			transform:rotateX(80deg);
		}
		ul li:nth-child(13){
			transform:rotateX(100deg);
		}
		ul li:nth-child(14){
			transform:rotateX(120deg);
		}
		ul li:nth-child(15){
			transform:rotateX(140deg);
		}
		ul li:nth-child(16){
			transform:rotateX(160deg);
		}


		section:nth-of-type(2){
			width:800px;
			height:800px;
			position:fixed;
			left:0;
			right:0;
			top:0;
			bottom:0;
			margin:auto;
			border-radius: 100%;
			transform:rotateX(70deg) rotateY(-20deg);
			
			transform-style: preserve-3d;
			animation: move1 20s linear infinite;
		}
		section:nth-of-type(2) ul{
			width:80px;
			height:80px;
			position:absolute;
			left:45%;
			top:-20px;
			transform-style: preserve-3d;
			animation: move2 10s linear infinite;
		}
		section:nth-of-type(2) ul li{
			width:100%;
			height:100%;
			border:1px solid blue;
			position:absolute;
			border-radius: 100%;
			box-shadow: 0 2px 20px blue;
		}


		section:nth-of-type(3){
			width:1200px;
			height:1200px;
			position:fixed;
			left:0;
			right:0;
			top:0;
			bottom:0;
			margin:auto;
			border-radius: 100%;
			transform:rotateX(70deg) rotateY(-20deg);
			
			transform-style: preserve-3d;
			animation: move1 17s linear infinite;
		}
		section:nth-of-type(3) ul{
			width:60px;
			height:60px;
			position:absolute;
			left:45%;
			top:-20px;
			transform-style: preserve-3d;
			animation: move2 10s linear infinite;
		}
		section:nth-of-type(3) ul li{
			width:100%;
			height:100%;
			border:1px solid yellow;
			position:absolute;
			border-radius: 100%;
			box-shadow: 0 2px 20px yellow;
		}
		section:nth-of-type(4){
			width:1500px;
			height:1500px;
			position:fixed;
			left:0;
			right:0;
			top:0;
			bottom:0;
			margin:auto;
			border-radius: 100%;
			transform:rotateX(70deg) rotateY(-20deg);
			
			transform-style: preserve-3d;
			animation: move1 25s linear infinite;
		}
		section:nth-of-type(4) ul{
			width:100px;
			height:100px;
			position:absolute;
			left:45%;
			top:-20px;
			transform-style: preserve-3d;
			animation: move2 15s linear infinite;
		}
		section:nth-of-type(4) ul li{
			width:100%;
			height:100%;
			border:1px solid #bf13ea;
			position:absolute;
			border-radius: 100%;
			box-shadow: 0 2px 20px #bf13ea;
		}
		section:nth-of-type(5){
			width:900px;
			height:900px;
			position:fixed;
			left:0;
			right:0;
			top:0;
			bottom:0;
			margin:auto;
			border-radius: 100%;
			transform:rotateX(60deg) rotateY(-50deg);
			
			transform-style: preserve-3d;
			animation: move3 25s linear infinite;
		}
		section:nth-of-type(5) ul{
			width:60px;
			height:60px;
			position:absolute;
			left:45%;
			top:-20px;
			transform-style: preserve-3d;
			animation: move2 3s linear infinite;
		}
		section:nth-of-type(5) ul li{
			width:100%;
			height:100%;
			border:1px solid #13ea32;
			position:absolute;
			border-radius: 100%;
			box-shadow: 0 2px 20px #13ea32;
		}
		/* 公转 */
		@keyframes move1{
			0%{transform:rotateX(70deg) rotateY(-20deg) rotateZ(0);}
			50%{transform:rotateX(70deg) rotateY(-20deg) rotateZ(180deg);}
			100%{transform:rotateX(70deg) rotateY(-20deg) rotateZ(360deg);}
		}
		/* 自转 */
		@keyframes move2{
			0%{transform:rotate(0);}
			50%{transform:rotate(180deg);}
			100%{transform:rotate(360deg);}
		}
		/* 公转2 */
		@keyframes move3{
			0%{transform:rotateX(60deg) rotateY(-50deg) rotateZ(0);}
			50%{transform:rotateX(60deg) rotateY(-50deg) rotateZ(180deg);}
			100%{transform:rotateX(60deg) rotateY(-50deg) rotateZ(360deg);}
		}
	</style>
</head>
<body>
	<section class="ball1">
		<ul>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
		</ul>
	</section>
	<section>
		<ul>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
		</ul>
	</section>
	<section>
		<ul>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
		</ul>
	</section>
	<section>
		<ul>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
		</ul>
	</section>
	<section>
		<ul>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
			<li></li>
		</ul>
	</section>
	<audio src="onlytime.mp3" autoplay loop></audio>
</body>
</html>
