target-listen
=============
Learning a thing or two about event target and add event listeners. It's baby steps to becoming a JS Ninja.
Adding EventTarget.addEventListener

<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Document</title>
</head>
<body>

	<table id="outside">
		<tr><td id="t1">one</td></tr>
		<tr><td id="t2">two</td></tr>
	</table>
	
</body>
<script type="text/javascript">
	function modifyText() {
		var t2 = document.getElementById("t2");
		if (t2.firstChild.nodeValue == "three") {
	    } else {
	    	t2.firstChild.nodeValue = "three";
	    }
    }

    var el = document.getElementById("outside");
    el.addEventListener("click", modifyText, false);
</script>
</html>
