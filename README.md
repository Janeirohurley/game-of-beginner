<!DOCTYPE html>
<html>
<head>
<title>authenticition</title>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width" />
<style type="text/css">
body{
margin: 0px;
height: 100vh;
background-image:url("gang/Sat.jpg");
background-attachment: fixed;
display:flex;
justify-content:center;
align-items:center;

}
form{
width: 400px;
background-color:rgba(0,0,0,0.3);
padding:60px;
box-sizing:border-box;

}
h1{
font-size: 18pt;
color:#fff;
border-bottom:solid 1px rgba(255,255,255,0.3);
}
.input{
padding:4px;
margin:10px 0;
background-color:transparent;
}
input {
color: yellow;
width: 90%;
border:none;
background: none;
outline: none;
}
.submit{
background-color:#41666c;
padding:6px 0;
text-align: center;
cursor:pointer;
color: #fff;
}
.submit:hover{
-webkit-filter:brightness(2.1);
}
.user{
position: absolute;
-webkit-transform: translate(-1000%)
}
.ht{
height:20px;
background-color:transparent;
}
.eyered{
position: absolute;
cursor: pointer;
left:240px;
-webkit-transform: translateY(-170%)
}
.lock{
position: relative;
-webkit-transform: translateY(-1475%);
top: 259px;
right:20px;
}
</style>
</head>
<body>
<form name="fo" method="hit.php">
<h1>autentifficaion</h1>
<div class="input">
<input type="text" name="E-mail or phone number" placeholder="login" />
<img src="gang/ccount.png" width="20" height="20" class="user" />
</div>
<div class="input">
<input type="password" class="ht" id="pass" name="pass" placeholder="password" />
</div>
<img src="gang/eyeoff.png" class="eyered" id="eye" width="20" height="20" onClick="f()" />
<img src="gang/lock.png" width="20" height="20" class="lock" />
<div  class="submit" onClick="document.fo.submit()">s'authentifier</div>
</form>
</body>

<script>
b=true;
function f(){
if(b)
{
document.getElementById("pass").setAttribute("type","text");
document.getElementById("eye").src="gang/eyered.png";
b=false;
}
else{

document.getElementById("pass").setAttribute("type","password");
document.getElementById("eye").src="gang/eyeoff.png";
b=true;
}
}

</script>
</html>
