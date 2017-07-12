# rotatepicture
用javascript +css3写的旋转相册
拖动鼠标
相册就能进行旋转
<h4>var e = e || window.event;<br/>			lastX = e.clientX;<br/>			lastY = e.clientY;	<br/>		this.onmousemove = function(e){			//鼠标移动	<br/>		var e = e || window.event;	<br/>		nowX = e.clientX;		<br/>	nowY = e.clientY;			//计算差	<br/>		minuX = nowX - lastX;<br/>			minuY = nowY - lastY;			//求旋转度数	<br/>		roY += minuX * 0.1;		<br/>	roX -= minuY * 0.2;		<br/>	owrap.style.transform = "rotateX("+roX+"deg) rotateY("+roY+"deg)";	<br/>		lastX = nowX;	<br/>	lastY = nowY;</h4>
