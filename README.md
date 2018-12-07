# sanjeev
purohith services
<html>
<head>
<script src="../src/panchang.js"></script>
<style>
.block{
  overflow:hidden;
}
.trow {
      display: table-row;
}
.alignL {
  text: bold;
}
.alignL, .alignR {
      display: table-cell;
      padding-right: 25px;
}
.alignR {
    margin: 1px 1px;
}
</style>
</head>
<body>
<h1>Sample app using PanchangJS:</h1>
<p>
 This sample code illustrates how to create a Panchang calendar using panchangJS javascript library.
</p>
<div class="trow">
<div class="alignL" >Day: </div><div id='day' class="alignR"></div>
</div>
<div class="trow">
<div class="alignL">Tithi: </div><div id=tithi class="alignR"></div>
</div>
<div class="trow">
<div class="alignL">Nakshtra: </div><div id=nakshtra class="alignR"></div>
</div>
<div class="trow">
<div class="alignL">Karna: </div><div id=karna class="alignR"></div>
</div>
<div class="trow">
<div class="alignL">Yoga: </div><div id=yoga class="alignR"></div>
</div>
<div class="trow">
<div class="alignL">Raasi: </div><div id=raasi class="alignR"></div>
</div>
<div class="trow">
<div class="alignL">Ayanamsa: </div><div id=ayanamsa class="alignR"></div>
</div>
<script>
  var t= new Date();
  panchang.calculate(t, function() {
    document.getElementById("day").innerHTML=panchang.Day.name;
    document.getElementById("tithi").innerHTML=panchang.Tithi.name;
    document.getElementById("nakshtra").innerHTML=panchang.Nakshatra.name;
    document.getElementById("karna").innerHTML=panchang.Karna.name;
    document.getElementById("yoga").innerHTML=panchang.Yoga.name;
    document.getElementById("raasi").innerHTML=panchang.Raasi.name;
    document.getElementById("ayanamsa").innerHTML=panchang.Ayanamsa.name;
  });
</script>
</body>
</html
