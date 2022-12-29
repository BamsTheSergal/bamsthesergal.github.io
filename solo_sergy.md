<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
</head>
<body>

<div style="text-align:center">
  <h2>Tabbed Image Gallery</h2>
  <p>Click on the images below:</p>
</div>

<!-- The four columns -->
<div class="row">
  <div class="column">
    <img src="1test.png" alt="test1" style="width:100%" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="2test.png" alt="test2" style="width:100%" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="3test.png" alt="test3" style="width:100%" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="4test.png" alt="test4" style="width:100%" onclick="myFunction(this);">
  </div>
</div>

<div class="container">
  <span onclick="this.parentElement.style.display='none'" class="closebtn">&times;</span>
  <img id="expandedImg" style="width:100%">
  <div id="imgtext"></div>
</div>

<script>
function myFunction(imgs) {
  var expandImg = document.getElementById("expandedImg");
  var imgText = document.getElementById("imgtext");
  expandImg.src = imgs.src;
  imgText.innerHTML = imgs.alt;
  expandImg.parentElement.style.display = "block";
}
</script>

</body>
</html>
