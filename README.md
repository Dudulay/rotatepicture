# rotatepicture
用javascript +css3写的旋转相册
拖动鼠标
相册就能进行旋转
<h4>var e = e || window.event;			lastX = e.clientX;			lastY = e.clientY;			this.onmousemove = function(e){			//鼠标移动			var e = e || window.event;			nowX = e.clientX;			nowY = e.clientY;			//计算差			minuX = nowX - lastX;			minuY = nowY - lastY;			//求旋转度数			roY += minuX * 0.1;			roX -= minuY * 0.2;			owrap.style.transform = "rotateX("+roX+"deg) rotateY("+roY+"deg)";			lastX = nowX;			lastY = nowY;</h4>
