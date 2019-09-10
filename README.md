# PersonalWeb
Personal web design
<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="utf-8">
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		<title>Jennie Florensia</title>
		<link href="https://fonts.googleapis.com/css?family=Nunito&display=swap" rel="stylesheet">
		<link rel="stylesheet" type="text/css" href="style.css">
	</head>
	<body class="black">
		<div class="center">
			<h1>Welcome to my website</h1>
			<h4 id="top">Minimalist - Stylish - Modern - Simplistic Design</h4>
		</div>
		<div>
			<nav class="col-5 padding-12 center bar">
				<ul>
					<li class="col-2"><a href="home.html"><img src="images/home-button.png" alt="Home"></a></li>
					<li class="col-2"><a href="aboutme.html">About Me</a></li>
					<li class="col-2"><a href="portfolio.html">Portfolio</a></li>
					<li class="col-2"><a href="gallery.html">Gallery</a></li>
				</ul>
			</nav>
		</div>
		<div class="slideshow-container">
			<div class="mySlides fade">
  				<img src="images/sld1.png" style="width:100%" alt ="slide1">
  			</div>

			<div class="mySlides fade">
  				<img src="images/sld2.png" style="width:100%" alt="slide2">
			</div>

			<div class="mySlides fade">
  				<img src="images/sld3.png" style="width:100%" alt="slide3">
			</div>
		</div>
		<br>

		<div style="text-align:center">
  			<span class="dot"></span> 
  			<span class="dot"></span> 
  			<span class="dot"></span> 
		</div>

		<script>
			var slideIndex = 0;
			showSlides();

			function showSlides() {
  				var i;
  				var slides = document.getElementsByClassName("mySlides");
  				var dots = document.getElementsByClassName("dot");
  				for (i = 0; i < slides.length; i++) {
    				slides[i].style.display = "none";  
  				}
  				slideIndex++;
  				if (slideIndex > slides.length) {slideIndex = 1}    
  				for (i = 0; i < dots.length; i++) {
    				dots[i].className = dots[i].className.replace(" active", "");
  				}
  				slides[slideIndex-1].style.display = "block";  
 				dots[slideIndex-1].className += " active";
  				setTimeout(showSlides, 3000); // Change image every 3 seconds
			}
		</script>
		<div class="col-5 padding-12 center conbox">
			<div class="tooltip">
				<a href="mailto:jennie@student.umn.ac.id"><img src="images/gmail.png" alt="gmail"></a>
				<span class="tooltiptext">jennie@student.umn.ac.id</span>
			</div>
			<div class="tooltip">
				<a href="http://line.me/ti/p/~jennie_florensia"><img src="images/line.png" alt="line"></a>
				<span class="tooltiptext">ID : jennie_florensia</span>
			</div>
			<div class="tooltip">
				<a href="https://instagram.com/tastelesstofu"><img src="images/ig.png" alt="ig"></a>
				<span class="tooltiptext">@tastelesstofu</span>
			</div>
		</div>
	</body>
	</html>
