
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.container {
  display: inline-block;
  cursor: pointer;
}

.personalInfo, .idealJob, .personalProfile, .projectIdea {
  width: 35px;
  height: 5px;
  background-color: #333;
  margin: 6px 0;
  transition: 0.4s;
}

.change .personalInfo {
  -webkit-transform: rotate(-45deg) translate(-9px, 6px);
  transform: rotate(-45deg) translate(-9px, 6px);
}

.change .idealJob {opacity: 0;}

.change .personalProfile {
  -webkit-transform: rotate(45deg) translate(-8px, -8px);
  transform: rotate(45deg) translate(-8px, -8px);
  
  .change .projectIdea {opacity: 0;}
}
</style>
</head>
<body>

<p>Click on the Menu Icon to transform it to "X":</p>
<div class="container" onclick="myFunction(this)">
  <div class="personalInfo"></div>
  <div class="idealJob"></div>
  <div class="personalProfile"></div>
  <div class="projectIdea"></div>
</div>

<script>
function myFunction(x) {
  x.classList.toggle("change");
}
</script>

</body>
</html>
