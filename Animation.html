<html>
<head>
<title>Hello</title>

<style>
	#myCanvas{
		background-color: rgb(99,184,255); 
		width: 500px;
		heigth: 500px; 
	}
</style>

<script>
	var c; 
	var ctx; 
	var s, circ, sta, spark, shap; 
	var s2, circ2, sta2, spark2, shap2; 

	var words = ["H", "e", "l", "l", "o"]; 
	var Letters = []; 

	var colors = ["CCCCFF", "#FFF68F", "#AB82FF", "#7FFFD4", "#FFB6C1", "#CAE1FF","#C0FF3E","#87CEFA","white"]; 


	var counter = 0; 
	var timer = 100; 

	var set = false; 

	var Letter = function(a, b, l, i){
		var x, y, dy;
		var name, num;  
		
		this.x = a; 
		this.y = b; 
		this.name = l; 
		this.dy = 0;
		this.num = i;

	}

	Letter.prototype.drawLetter = function(){
		ctx.font = "30px Arial"; 
		ctx.fillStyle = "white";
		ctx.fillText(this.name, this.x, this.y); 
	}

	Letter.prototype.moveLetter = function(){
		this.y += this.dy; 
	}

	function checkCollison(l){

		switch(l.name){
			case "H":

				if(l.y <= s.y + s.height) 
					l.dy = 5; 
				break; 
			case "e":
				if(l.y <= circ.y + circ.radius)
					l.dy = 5; 
				break; 
			case "l": 
				if(l.y <= sta.y && l.x == sta.x)
					l.dy = 5; 
				else if(l.y <= spark.y + spark.width && l.x == spark.x)
					l.dy = 5; 
				break; 
			case "o": 
				if(l.y <= shap.y + shap.width && l.x == shap.x)
					l.dy = 5; 
				break; 
		}
	}

	var Square = function(x, color){
		var x, y, dy; 
		var width, height; 
		var color; 

		this.x = x; 
		this.y = 0; 
		this.dy = 2; 

		this.width = 20; 
		this.height = 20; 

		this.color = color; 
	}

	Square.prototype.drawSquare = function(){
		ctx.fillStyle = this.color; 
		ctx.beginPath(); 
		ctx.fillRect(this.x, this.y, 20, 20); 
		ctx.closePath(); 
	}

	Square.prototype.moveSquare = function(){
		this.y += this.dy; 
	}

	var Circle =  function(x, color){
			var x, y, dy;
			var width, height; 
			var color; 

			this.x = x;
			this.y = -80;
			this.dy = 2; 
			
			this.radius = 10;
			this.color = color;  
		}
		
	Circle.prototype.drawCircle = function() {
		var c=document.getElementById("myCanvas");
		var ctx=c.getContext("2d");
		ctx.beginPath();
		ctx.arc(140,this.y,10,0,2*Math.PI);
		ctx.fillStyle = this.color;
		ctx.fill();
	}

	Circle.prototype.moveCircle = function(){
		this.y += this.dy; 
	}
		
	var Star = function(x, color){
		var x, y, dy; 
		var width, height; 
		var spikes, outerRadius, innerRadius;
		var color;

		this.x = x; 
		this.y = -160; 
		this.dy = 2;

		this.width = 10; 
		this.height = 20; 
		
		this.spikes = 5; 
		this.outerRadius = 10; 
		this.innerRadius = 15; 
		this.color = color; 
	}

	Star.prototype.drawStar = function () {
	    var rot = Math.PI / 2 * 3;
	    var x = this.x;
	    var y = this.y;
	    var step = Math.PI / this.spikes;

	    ctx.beginPath();
	    ctx.moveTo(this.x, this.y - this.outerRadius)
	    for (i = 0; i < this.spikes; i++) {
	        x = this.x + Math.cos(rot) * this.outerRadius;
	        y = this.y + Math.sin(rot) * this.outerRadius;
	        ctx.lineTo(x, y)
	        rot += step

	        x = this.x + Math.cos(rot) * this.innerRadius;
	        y = this.y + Math.sin(rot) * this.innerRadius;
	        ctx.lineTo(x, y)
	        rot += step
	    }
	    ctx.lineTo(this.x, this.y - this.outerRadius)
	    ctx.closePath();
	    ctx.fillStyle = this.color;
	    ctx.fill();
	}

	Star.prototype.moveStar = function(){
		this.y += this.dy; 
	}

	var Sparkle = function(x, color){
		var x, y, dy; 
		var width, height; 
		var spikes, outerRadius, innerRadius; 
		var color; 

		this.x = x; 
		this.y = -200; 
		this.dy = 2; 
		
		this.width = 10; 
		this.height = 10; 
		
		this.spikes = 20; 
		this.outerRadius = 10; 
		this.innerRadius = 15; 
		this.color = color;
		}

	Sparkle.prototype.drawSparkle = function () {
	    var rot = Math.PI / 2 * 3;
	    var x = this.x;
	    var y = this.y;
	    var step = Math.PI / this.spikes;

	    ctx.beginPath();
	    ctx.moveTo(this.x, this.y - this.outerRadius)
	    for (i = 0; i < this.spikes; i++) {
	        x = this.x + Math.cos(rot) * this.outerRadius;
	        y = this.y + Math.sin(rot) * this.outerRadius;
	        ctx.lineTo(x, y)
	        rot += step

	        x = this.x + Math.cos(rot) * this.innerRadius;
	        y = this.y + Math.sin(rot) * this.innerRadius;
	        ctx.lineTo(x, y)
	        rot += step
	    }
	    ctx.lineTo(this.x, this.y - this.outerRadius)
	    ctx.closePath();
	    ctx.fillStyle = this.color;
	    ctx.fill();

	}

	Sparkle.prototype.moveSparkle = function(){
		this.y += this.dy; 
	}

	var Shape = function(x, color){
		var x, y, dy; 
		var width, height; 
		var spikes, outerRadius, innerRadius;

		this.x = x; 
		this.y = -250; 
		this.dy = 2;

		this.width = 20; 
		this.height = 20; 
		
		this.spikes = 5; 
		this.outerRadius = 10; 
		this.innerRadius = 15; 

		this.color = color; 
	}

	Shape.prototype.drawShape = function () {
	    var rot = Math.PI / 2 * 3;
	    var x = this.x;
	    var y = this.y;
	    var step = Math.PI / this.spikes;

	    ctx.beginPath();
	    ctx.moveTo(this.x, this.y - this.outerRadius);
	    for (i = 0; i < this.spikes; i++) {
	        x = this.x + Math.cos(rot) * this.outerRadius;
	        y = this.y + Math.sin(rot) * this.outerRadius;
	        ctx.lineTo(x, y)
	        rot += step

	        x = this.x + Math.cos(rot) * this.innerRadius;
	        y = this.y + Math.sin(rot) * this.innerRadius;
	        ctx.lineTo(x, y)
	        rot += step
	    }
	    ctx.lineTo(this.x, this.y - this.outerRadius)
	    ctx.closePath();
	    ctx.fillStyle = this.color;
	    ctx.fill();

	}

	Shape.prototype.moveShape = function(){
		this.y += this.dy; 
	}

	function init(){
		c = document.getElementById("myCanvas"); 
		ctx = c.getContext("2d"); 

		createLetters();  

		s = new Square(100, colors[randInt(0, 7)]); 
		circ = new Circle(140, colors[randInt(0, 7)]);
		sta = new Star(180, colors[randInt(0, 7)]); 
		spark = new Sparkle(220, colors[randInt(0, 7)]);
		shap = new Shape(260, colors[randInt(0, 7)]); 

		s2 = new Square(100, colors[randInt(0, 7)]); 
		circ2 = new Circle(140, colors[randInt(0, 7)]);
		sta2 = new Star(180, colors[randInt(0, 7)]); 
		spark2 = new Sparkle(220, colors[randInt(0, 7)]);
		shap2 = new Shape(260, colors[randInt(0, 7)]);

		setInterval(draw, 10); 
	}

	function createLetters(){

		var i = 0; 

		x = 100; 

		while(i < 5){
			Letters.push(new Letter(x, 250, words[i], i)); 

			i++; 
			x = x + 40; 
		}
	}

	function checkOffScreen(){
		if(s.y > c.width)
			s = new Square(randInt(0, 500), colors[randInt(0, 7)] 	); 

		if(circ.y >c.width)
			circ = new Circle(randInt(0, 500), colors[randInt(0, 7)]);

		if(sta.y > c.width)
			sta = new Star(randInt(0, 500), colors[randInt(0, 7)]); 
		
		if(spark.y > c.width)
			spark = new Sparkle(randInt(0, 500), colors[randInt(0, 7)]);
		
		if(shap.y > c.width)
			shap = new Shape(randInt(0, 500), colors[randInt(0, 7)]);

		if(s2.y > c.width)
			s2 = new Square(randInt(0, 500), colors[randInt(0, 7)]); 

		if(circ2.y > c.width)
			circ2 = new Circle(randInt(0, 500), colors[randInt(0, 7)]);

		if(sta2.y > c.width)
			sta2 = new Star(randInt(0, 500), colors[randInt(0, 7)]); 
		
		if(spark2.y > c.width)
			spark2 = new Sparkle(randInt(0, 500), colors[randInt(0, 7)]);
		
		if(shap2.y > c.width)
			shap2 = new Shape(randInt(0, 500), colors[randInt(0, 7)]);
	}
	var y = 0; 
	 

	function draw(){
		
		clear(); 

		s.drawSquare(); 
		s.moveSquare(); 
		
		circ.drawCircle(); 
		circ.moveCircle();
		
		sta.drawStar(); 
		sta.moveStar();
		
		spark.drawSparkle(); 
		spark.moveSparkle();
		
		shap.drawShape(); 
		shap.moveShape(); 

		if(timer <= 0){

			s2.drawSquare(); 
			s2.moveSquare(); 
			
			circ2.drawCircle(); 
			circ2.moveCircle();
			
			sta2.drawStar(); 
			sta2.moveStar();
			
			spark2.drawSparkle(); 
			spark2.moveSparkle();
			
			shap2.drawShape(); 
			shap2.moveShape(); 
		}
		
		y++;
		
		var i = 0; 
		while(i < 5){
			var temp = Letters[i];

			temp.drawLetter(); 
			checkCollison(temp); 
			temp.moveLetter(); 

			i++; 
		}

		timer--; 
		checkOffScreen(); 
	}

	function clear(){
		ctx.clearRect(0,0,500,500); 
	}

	function randInt(min, max){
		return Math.floor(Math.random() * (min, max) + min); 
	}


</script>
</head>
<body onLoad="init()">
<canvas id="myCanvas" width="500" height="500" ></canvas>
</body>
</html>