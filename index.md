<html>
<head>
<script language='JScript'>
function GetRandString(n) {
     var res = "";
     var chars = ['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z'];
     for(var i = 0; i < n ; i ++) {
         var id = Math.ceil(Math.random()*51);
         res += chars[id];
     }
     return res;
 }
 function Renew(){
 	var ms="";
 	var cN=document.getElementById("num").value || 8;
 	ms=GetRandString(cN);
 	xID=document.getElementById("ipb");
 	xID.value=ms;
 	}
</script>
</head>
<body><center><font color=blue><h1>这是一个随机字符串生成器,</h1></font><textarea id="ipb" rows="5" cols="50">请单击‘生成’按钮生成随机字符串！</textarea><br><br><font color=red>字符串长度： </font><input id="num" value="8">  <button type="button" onclick="Renew()">生成</button></center>
</body>
</html>
