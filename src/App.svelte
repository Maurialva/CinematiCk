<script>
	
	import CustomButton from './CustomButton.svelte';
	
let src = 'logocinematick.jpg';
	let namel = 'logo';
function handleClick() {
	location.href='login.html';
	
}import CustomB from './ButtonSubscribe.svelte';
</script>
<body>

<main>
<div id="header">
	<div align="right">
	<!-- {src} is short for src={src} -->
	<img align="left" {src} alt="{namel}" class="logo" height="90" width="170" vertical-align="top" >
	<a  href="https://www.instagram.com/"> <img  class= "socialicon" src="logo_instagram.png"  alt="Instagram" height="60" width="60"></a>
	<a href="https://www.facebook.com/"> <img class= "socialicon" src="logo_facebook.png" alt="Facebook" height="60" width="60"></a>
	<a href="https://www.twitter.com/"> <img  class= "socialicon"src="logo_twitter.png" alt="Twitter" height="60" width="60"></a>
	<CustomButton on:click={handleClick} /> 
	<br><br>
	<br>
	</div>
	<div class="search-container">
		
		<br>
		<form action="http://localhost:5000/">
			
		<input type="text" placeholder="Buscar..." name="searchbar"  >
		
		<input type="image" src="icon_search1.png"alt="Submit"  />
		<br>
		<br>
		</form>
		
	</div>
	
</div>
</main>
<left>
	<div id="cartelera">
		<h2>Cartelera</h2> 
		<a href="https://www.instagram.com/"> <img class="responsive" src="p_sample.jpg" alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img class="responsive" src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img  class="responsive"src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		<br><br>
		<a href="https://www.instagram.com/"> <img class="responsive" src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img class="responsive" src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img class="responsive" src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		<br><br>
		<a href="https://www.instagram.com/"> <img class="responsive" src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img class="responsive" src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img class="responsive" src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		
	
	</div>

</left>
<right>
	<div id="suscripcion">
<h2>Suscribirse</h2>
<input type="text" placeholder="Email..." name="suscrip"  ><br>
<CustomB on:click={handleClick} /> 
	</div>
	<div id="destacada">
		<h2>destacada</h2>
		<figure >
		<a href="https://www.instagram.com/"> <img class="destacada" src="p_sample.jpg" alt="Instagram" height="300" width=""></a>
		<figcaption>TITULO</figcaption>
	</figure>
	</div>
</right>
<footer>
	<a class="foot" href="http://localhost:5000/"> INICIO</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	<a class="foot"  href="http://localhost:5000/"> SOBRE NOSOTROS</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	<a class="foot" href="http://localhost:5000/"> CONTACTO</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	<a class="foot" href="http://localhost:5000/"> AYUDA</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</footer>
</body>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		background-color: black;
		width: 90%;
	}
	
	body {
		text-align: center;
		padding: 1em;
		max-width: 1200px;
		margin: 0 auto;
		background-color: black;
		
	}
	@media screen and (min-width: 240px) {
		main {
			max-width: none;
			font-size: 80%;
		}
		right{
			font-size: 100%;
		}
		left
		{
			font-size: 100%;	
			width: 30%;
  		
  		height: auto;
		}
		footer {
			font-size: 100%;

		}
		input[type=text] 
		{
			font-size: 150%;
		}
		.responsive{
			width: 30%;
  		
  		height: auto;
		}

	}

	@media screen and (max-width: 600px) {
  
		main {
			max-width: none;
			font-size: 25%;
		}
		right{
			font-size: 25%;
			padding: 0.5%;
			margin: 0.5%;
			border: 2px;
			height: auto;
		}
		left
		{
			font-size: 25%;
			width: 30%;
			padding: 0.5%;
			margin: 0.5%;
			border: 2px ;
  		height: auto;
		}
		footer {
			font-size: 25%;

		}
		input[type=text] 
		{
			font-size: 50%;
		}
		.responsive{
			width: 20%;
  		
  		height: auto;
		}
	}
	:global(h1)
	{
		color: #750c0c;
		text-transform: uppercase;
		font-size: 25px;
		font-weight: 100;
	}
	:global(h2)
	{
		vertical-align:middle;
		color: #750c0c;
		text-transform: uppercase;
		font-size: 200%;
		font-weight: 10;
		text-align: center;
	}
	.search-container
	{
		text-align: center;
		width: 100%;
		background-image: linear-gradient(rgb(65, 9, 9) 0%, rgb(158, 80, 80) 56%, rgb(54, 12, 12) 100%); 
		border-radius: 50px;
		
	}
	input[type=text] 
	{
		vertical-align:middle;
		text-align: center;
		transition: background 900ms ease-in-out;
		background-color: rgb(90, 29, 29);
		background-position: 100%;
		background-size: 200%;
		border: brown;
		background-image: linear-gradient(90deg,rgb(17, 12, 12) 0%, rgb(75, 21, 21) 56%, rgb(70, 17, 17) 100%);		
		color: rgb(255, 255, 255); 
		border-radius: 50px; 
		width:80%;
		}
	
	input:focus {  border-image: #000000; 
	outline: none;
	background-position: 0;
	transition: background 900ms ease-in-out;
	background-image: linear-gradient(43deg,rgb(0, 0, 0) 0%, rgb(37, 26, 26) 56%, rgb(39, 4, 4) 100%); 
	}
	input:hover{
		background-position: 0;
		transition: background 900ms ease-in-out;
		background-image: linear-gradient(43deg,rgb(0, 0, 0) 0%, rgb(37, 26, 26) 56%, rgb(39, 4, 4) 100%); 
	}
	input[type=image]{

		width: 6%;
  		
  		height: auto;
	border: none;
	cursor: pointer;
	vertical-align:middle;
	}
	#header
	{
		background-color: black;
		width: 100%;
		
	}
	#cartelera
	{
	float: left;
	align-self: left;
	text-align: left;
	border: 4px solid rgb(65, 9, 9);
	border-radius: 50px;
	width: 53%;
	padding: 1%;
	margin: 1%;
	text-align: center;
	}
	#suscripcion
	{
		float: right;
	align-self: center;
	text-align: center;
	border: 4px solid rgb(65, 9, 9);
	border-radius: 50px;
	width: 25%;
	padding: 1%;
	margin: 1%;
	}
	#destacada
	{
		float: right;
	align-self: center;
	text-align: center;
	border: 5px solid rgb(65, 9, 9);
	border-radius: 50px;
	width: 25%;
	padding: 1%;
	margin: 1%;
	}
	:global(figure)
	{
		
	align-self: center;
	text-align: center;
	margin: 10px;
		
	}
	figcaption {
		vertical-align:middle;
		color: #750c0c;
		text-transform: uppercase;
		font-size: 1em;
		font-weight: 10;
}
	footer
	{
		background-image: linear-gradient(rgb(65, 9, 9) 0%, rgb(158, 80, 80) 50%, rgb(54, 12, 12) 100%);
	float:left;
	align-self: center;
	text-align: center;
	
	border-radius: 50px;
	width: 100%;
	padding: 1%;
	margin: 1%;
	
	}

	.responsive
	{
  		height: auto;
	}
	.destacada
	{
		width: 80%;
  		
  		height: auto;
	}
	.socialicon
	{
		width: 6%;
  		
  		height: auto;
	}
	.logo
	{
		width: 17%;
  		
  		height: auto;
	
	}
	
</style>
