# Jasipro-
Codepro
<!DOCTYPE html>
<html>
<head>
	<title>Registration Form</title>
</head>
<body>
	<form id="registrationForm">
		<label for="firstName">First Name:</label>
		<input type="text" id="firstName" name="firstName"><br><br>
		<label for="lastName">Last Name:</label>
		<input type="text" id="lastName" name="lastName"><br><br>
		<label for="email">Email:</label>
		<input type="email" id="email" name="email"><br><br>
		<label for="contact">Contact:</label>
		<input type="tel" id="contact" name="contact"><br><br>
		<label for="address">Address:</label>
		<input type="text" id="address" name="address"><br><br>
		<label for="city">City:</label>
		<input type="text" id="city" name="city"><br><br>
		<button id="registerButton">Register</button>
	</form>

	<script src="script.js"></script>
</body>
</html>





const form = document.getElementById('registrationForm');
const registerButton = document.getElementById('registerButton');

registerButton.addEventListener('click', function(event) {
	event.preventDefault();
	if (form.checkValidity()) {
		alert('Registration Completed!');
		// Form submission logic here
	} else {
		alert('Please fill out all required fields!');
	}
});
