<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8" />
<title>RolldDice</title>
<link rel="stylesheet" href="Puzzle_1style.css"/>
<script type="text/javascript">
function f1() {
 var a=parseInt(document.getElementById("ans").value);
 if (a==2){alert("Congrats! Right answer");}
 else{alert("Oops! Wrong answer.");}
 }
function f2(){
var total = 0
for (var i = 0; i < 4; i++) { 
  var random = Math.round(Math.random()*4) + 1;
  document.getElementById("myImg" + i.toString()).src = "C:/Users/ELVIS/Desktop/rollDice/petals/dice-" + random.toString() + ".png";
  if (random == 2) {
 total += 2
}
  if (random == 4) {
 total += 4
}

}
document.getElementById("totalpetals").innerHTML= 'There are '+total+' petals around the rose. ';

}

</script>
</head>
<body>
<center>
<h1> PETALS 'ROUND THE ROSE </h1>
<div id = "rules"><p> The rules require that you roll the dice below and then answer correctly "how many petals there are around the rose". </p>
<p>You can repeat the procedure until you discover the secret rule of the puzzle or you can give up.
How many throws do you need to figure out this puzzle? </p></div>
<div id = "petalaroundtherose">
<div id = "dicepetals" class = "aligncenter is-resized" style = "width:100%">
<div id = "petal-die" style = "display: inline-block">
<img id = "myImg0" src="C:\Users\ELVIS\Desktop\rollDice\petals\dice-1.png" width="90" height = "90" name="dice-1"> 
</div>
<div id = "petal-die" style = "display: inline-block">
<img id = "myImg3" src="C:\Users\ELVIS\Desktop\rollDice\petals\dice-2.png" width="90" height = "90" name="dice-2">
</div>
<div id = "petal-die" style = "display: inline-block">
<img id = "myImg1" src="C:\Users\ELVIS\Desktop\rollDice\petals\dice-3.png" width="90" height = "90" name="dice-3">
</div>
<div id = "petal-die" style = "display: inline-block">
<img id = "myImg2" src="C:\Users\ELVIS\Desktop\rollDice\petals\dice-4.png" width="90" height = "90" name="dice-4">
</div>
</div>
<div id ="totalpetals"> There are 6 petals around the rose. </div>
<img id ="rolld" src="C:\Users\ELVIS\Desktop\rollDice\rollme.jpg" width="60" height="60" onclick="f2()">
</div>
<div id="ddd">
<p> Text the number in the given box and submit if you think your answer is right. Go for it!</p></div>
</div id= "yourquestion">
<div id= "quest-die" style = "display: inline-block">
<img src = "C:\Users\ELVIS\Desktop\rollDice\petals\dice-2.png" width="80" height = "80" > </div>
<div id= "quest-die" style = "display: inline-block">
<img src = "C:\Users\ELVIS\Desktop\rollDice\petals\dice-5.png" width="80" height = "80" > </div>
<div id= "quest-die" style = "display: inline-block">
<img src = "C:\Users\ELVIS\Desktop\rollDice\petals\dice-0.png" width="80" height = "80" > </div>
<div id= "quest-die" style = "display: inline-block">
<img src = "C:\Users\ELVIS\Desktop\rollDice\petals\dice-1.png" width="80" height = "80"> </div>
<div id= "youranswer" >
Enter your answer: <input type = number id = ans size = 3><br><br>
<input type = "button" value = "SUBMIT" onclick="f1()"><br><br><br><br>
</div>
</center>
</body>
