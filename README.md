<!DOCTYPE html>
<html>
<body>

<canvas id="myCanvas" width="300" height="300" style="border:5px solid #000000;">
Your browser does not support the HTML canvas tag.</canvas>

<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
var n = 6;
for (let i = 0; i < n; i++) {
	ctx.moveTo(i/n*(c.width),0);
	ctx.lineTo(i/n*(c.width),c.height);
    
    ctx.moveTo(0,i/n*(c.width));
	ctx.lineTo(c.height,i/n*(c.width));
	ctx.stroke();
}
</script>
</body>
</html>
