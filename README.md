# <!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Fizz Buzz</title>
<script>

// Edited by: Brett McElvain 
// Date: 10/13/2022
// Course: INFOTC1000
// Challenge: FizzBuzz in JavaScript in Browser

function fizzbuzz() {
	var display = document.getElementById('display');
	var displayHTML = "";
	for (i = 1; i <= 100; i++) {
		// prints 'FizzBuzz' if divisible by 3 and 5.
		if (i%3 === 0 && i%5 === 0){
			displayHTML += "<p>" + 'FizzBuzz' + "</p>";
		
		} 
		// prints 'Fizz' if divisible by 3. 
		else if (i%3 === 0){
			displayHTML += "<p>" + 'Fizz' + "</p>";
		} 
		// prints 'Buzz' if divisible by 5.
		else if (i%5 === 0){
			displayHTML += "<p>" + 'Buzz' + "</p>";
		} 
		// prints 'current number' if not divisible by 3 and/or 5.
		else {
			displayHTML += "<p>" + i + "</p>";
		}
	}
	display.innerHTML = displayHTML
}

</script>

<header>
    <h1>Hello, INFOTC1000</h1>
    <p>----------Brett McElvain-----------</p>
    <p>----Thank you for stopping by!-----</p>
  </header>
<body onload="fizzbuzz()">
<div id="display">

</div>
</body>

</html>
