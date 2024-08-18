#tril for learn
html code for crete an object
<html>
<head>
	<title>Motion Example</title>
	<link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
	<div class="motion-container">
		<div class="moving-object"></div>
	</div>
	<script src="script.js"></script>
</body>
</html>
//css file
.motion-container {
	width: 100%;
	height: 100vh;
	overflow: hidden;
	position: relative;
}

.moving-object {
	width: 50px;
	height: 50px;
	background-color: red;
	position: absolute;
	animation: move 5s infinite;
}

@keyframes move {
	0% {
		transform: translateX(0);
	}
	50% {
		transform: translateX(300px);
	}
	100% {
		transform: translateX(0);
	}
}