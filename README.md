<html>
<head>
<title>Kalkulator</title> 
</head>
<body>
	 <center>
    <h1>Aplikasi Kalkulator Sederhana</h1>
    </center>
  <style type="text/css">
    body{
      background-color: black;
      font-style: italic;
      color: white;
    }
  </style>
<script language="JavaScript" type="text/javascript">

<!--
//Source code java script untuk membuat perklalian, pengurangan, penjumlahan dan pembagian menggunakan if else
function hitung(){

var kalkulator = document.form1;
var x=eval(kalkulator.x.value);
var y=eval(kalkulator.y.value);
var pil= kalkulator.opt.value;
if (pil == "di tambah") {
var z = x + y;
 }else if (pil == "di kurang") {
var z = x - y;
 } else if (pil == "di kali") {
var z = x * y;
 } else if (pil == "di bagi") {
var z = x / y;
 }
 kalkulator.hasil.value = z;
 kalkulator.x.value = "";
 kalkulator.y.value = "";
}
function resetForm(){
document.form1.reset();
}

//-->

</script>
<div align="center">
<form name="form1" action="#">
<p>bil 1  <input type="text" name="x" /></p>
<p>bil 2  <input type="text" name="y" /></p>
<p>hasil  <input type="text" name="hasil" disabled="true" /></p>
<p>operator <select name="opt"></p>
 <option value="tambah"> + (di tambah)</option>
 <option value="kurang"> - (di kurang)</option>
 <option value="kali"> * (di kali)</option>
 <option value="bagi"> / (di bagi)</option>
</select>
<input type="button" value="=" onClick="hitung()" />
<input type="button" value="CLEAR" onClick="resetForm()" />
</form>
</body>
</html>
