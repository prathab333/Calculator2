# Calculator2
k!
<!DOCTYPE HTML>
<html>
<title>Calculator</title>
<style>
body
{
	margin:2px;
}
.box
{
	font-family:agency FB;
	font-size:20px;
	background-color:#332e2e;
	color:white;
}
.buttons
{
	font-family:agency FB;
	font-size:18px;
	color:white;
	background-color:#332e2e;
}
.fc
{
	height:50px;
	postion:absolute;
	font-size:45px;
	font-family:agency FB;
	color:#00b0e5;
	text-align:center;
}
</style>
<body background="b (24).jpg">
<p class="fc">Simple Calculator<br>Enter 2 numbers and an operator at a time and proceed with further calculations..!</p>
<script>
function func7()
{
	var x = document.getElementById("b7").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function func8()
{
	var x = document.getElementById("b8").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function func9()
{
	var x = document.getElementById("b9").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function func4()
{
	var x = document.getElementById("b4").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function func5()
{
	var x = document.getElementById("b5").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function func6()
{
	var x = document.getElementById("b6").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function func1()
{
	var x = document.getElementById("b1").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function func2()
{
	var x = document.getElementById("b2").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function func3()
{
	var x = document.getElementById("b3").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function func0()
{
	var x = document.getElementById("b0").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function funcdiv()
{
	var x = document.getElementById("bdiv").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function funclear()
{
	document.getElementById("pp").value=0;
}
function funcmul()
{
	var x = document.getElementById("bmul").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function funcmod()
{
	var x = document.getElementById("bmod").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function funcrec()
{	
	var y=document.getElementById("pp").value;
	var z=1/y;
	document.getElementById("pp").value= z;
}
function funcsub()
{
	var x = document.getElementById("bsub").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function funcpoint()
{
	var x = document.getElementById("bpoint").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function funcadd()
{
	var x = document.getElementById("badd").value;	
	var y=document.getElementById("pp").value;
	document.getElementById("pp").value= y.concat("",x);
}
function funceq()
{
	var text= document.getElementById("pp").value;
	var len= text.length;
	var i,c,count=0;
	for(i=0;i<len;i++)
	{
		var temp=text.charAt(i);
		if(temp=='+' ||temp=='-'||temp=='*' ||temp=='/' || temp=='%')
		{
			count++;
			var a=text.substr(0,i);
			var aa=parseFloat(a);
			var b=text.substr(i+1,len);
			var bb=parseFloat(b);
			if(temp=='+')
				c=aa+bb;
			if(temp=='-')
				c=aa-bb;
			if(temp=='*')
				c=aa*bb;
			if(temp=='%')
				c=aa%bb;
			if(temp=='/')
				c=aa/bb;
			break;
		}
	}
	document.getElementById("pp").value=c;
}
</script>

<br><br><br><br><br><br>

<input class="box" type="text" id="pp" style="postion:relative;margin-top:0px;margin-left:450px;width:250px;height:35px">

<br><br>
<button class="buttons" id="b7"  value="7" onclick="func7()" style="position:absolute;margin-top:30px;margin-left:450px;height:50px; width:50px;"> 7 </button>
<button class="buttons" id="b8"  value="8" onclick="func8()" style="position:absolute;margin-top:30px;margin-left:500px;height:50px; width:50px"> 8 </button>
<button class="buttons" id="b9"  value="9" onclick="func9()" style="position:absolute;margin-top:30px;margin-left:550px;height:50px; width:50px"> 9 </button>
<button class="buttons" id="bdiv"  value="/" onclick="funcdiv()" style="position:absolute;margin-top:30px;margin-left:600px;height:50px; width:50px"> / </button>
<button class="buttons" id="bclear"  value="clear" onclick="funclear()" style="position:absolute;margin-top:30px;margin-left:650px;height:50px; width:50px"> clear </button>
<br>
<button class="buttons" id="b4"  value="4" onclick="func4()" style="position:absolute;margin-top:80px;margin-left:450px;height:50px; width:50px"> 4 </button>
<button class="buttons" id="b5"  value="5" onclick="func5()" style="position:absolute;margin-top:80px;margin-left:500px;height:50px; width:50px"> 5 </button>
<button class="buttons" id="b6"  value="6" onclick="func6()" style="position:absolute;margin-top:80px;margin-left:550px;height:50px; width:50px"> 6 </button>
<button class="buttons" id="bmul" value="*" onclick="funcmul()" style="position:absolute;margin-top:80px;margin-left:600px;height:50px; width:50px"> * </button>
<button class="buttons" id="bmod"  value="%" onclick="funcmod()" style="position:absolute;margin-top:80px;margin-left:650px;height:50px; width:50px"> % </button>
<br>
<button class="buttons" id="b1"  value="1" onclick="func1()" style="position:absolute;margin-top:130px;margin-left:450px;height:50px; width:50px"> 1 </button>
<button class="buttons" id="b2"  value="2" onclick="func2()" style="position:absolute;margin-top:130px;margin-left:500px;height:50px; width:50px"> 2 </button>
<button class="buttons" id="b3"  value="3" onclick="func3()" style="position:absolute;margin-top:130px;margin-left:550px;height:50px; width:50px"> 3 </button>
<button class="buttons" id="bsub"  value="-" onclick="funcsub()" style="position:absolute;margin-top:130px;margin-left:600px;height:50px; width:50px"> - </button>
<button class="buttons" id="brec"  value="rec" onclick="funcrec()" style="position:absolute;margin-top:130px;margin-left:650px;height:50px; width:50px"> 1/x </button>
<br>
<button class="buttons" id="b0"  value="0" onclick="func0()" style="position:absolute;margin-top:180px;margin-left:450px;height:50px; width:100px"> 0 </button>
<button class="buttons" id="bpoint"  value="." onclick="funcpoint()" style="position:absolute;margin-top:180px;margin-left:550px;height:50px; width:50px"> . </button>
<button class="buttons" id="badd"  value="+" onclick="funcadd()" style="position:absolute;margin-top:180px;margin-left:600px;height:50px; width:50px"> + </button>
<button class="buttons" id="beq"  value="=" onclick="funceq()" style="position:absolute;margin-top:180px;margin-left:650px;height:50px; width:50px"> = </button>

</body>
</html>
