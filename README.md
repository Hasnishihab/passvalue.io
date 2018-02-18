<html>
<body>

lattitude: <input type="text" id="lat" value="22.145"><br>
longitude: <input type="text" id="lng" value="55.0124">

<p>Click the button to display the value of the text field.</p>

<button onclick="myFunction()">Try it</button>
<div id="lattitude"></div>
<div id="longitude"></div>
<script>
function myFunction() {
    var la=lat.value;
	document.getElementById("lattitude").innerHTML = la;
	var ln=lng.value;
	document.getElementById("longitude").innerHTML = ln;
	if (typeof(Storage) !== "undefined") {
    // Store
    localStorage.setItem("lattitude", la);
	localStorage.setItem("longitude", ln);}
} 
</script>

</body>
</html>
