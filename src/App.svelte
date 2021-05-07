<script>
	
	import CustomButton from './CustomButton.svelte';
	
let src = 'logocinematick.jpg';
	let namel = 'logo';
function handleClick() {
	alert('clicked');
	
}import CustomB from './ButtonSubscribe.svelte';
</script>
<body>

<main>
<div id="header">
	<div align="right">
	<!-- {src} is short for src={src} -->
	<img align="left" {src} alt="{namel}" height="90" width="170" vertical-align="top" >
	<a href="https://www.instagram.com/"> <img  src="logo_instagram.png"  alt="Instagram" height="60" width="60"></a>
	<a href="https://www.facebook.com/"> <img  src="logo_facebook.png" alt="Facebook" height="60" width="60"></a>
	<a href="https://www.twitter.com/"> <img  src="logo_twitter.png" alt="Twitter" height="60" width="60"></a>
	<CustomButton on:click={handleClick} /> 
	<br><br>
	</div>
	<div class="search-container">
		
		<br>
		<form action="http://localhost:5000/">
			
		<input type="text" placeholder="Buscar..." name="searchbar" size="80%" >
		
		<input type="image" src="icon_search1.png"alt="Submit"  />
		<br>
		<br>
		</form>
		
	</div>
	
</div>
</main>
<left>
	<div id="cartelera">
		<h2>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
			&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
			&nbsp;
			&nbsp;&nbsp;&nbsp;
			&nbsp;&nbsp;Cartelera</h2> 
		<a href="https://www.instagram.com/"> <img  src="p_sample.jpg" alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img  src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img  src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		<br><br>
		<a href="https://www.instagram.com/"> <img  src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img  src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img  src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		<br><br>
		<a href="https://www.instagram.com/"> <img  src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img  src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		&nbsp;&nbsp;&nbsp;&nbsp;
		<a href="https://www.instagram.com/"> <img  src="p_sample.jpg"  alt="Instagram" height="300" width=""></a>
		
	
	</div>

</left>
<right>
	<div id="suscripcion">
<h2>Suscribirse</h2>
<input type="text" placeholder="Email..." name="suscrip"  >
<CustomB on:Click={handleClick} /> 
	</div>
	<div id="destacada">
		<h2>destacada</h2>
		<figure >
		<a href="https://www.instagram.com/"> <img  src="p_sample.jpg" alt="Instagram" height="300" width=""></a>
		<figcaption>TITULO</figcaption>
	</figure>
	</div>
</right>
<div id="footer">
	<a href="http://localhost:5000/"> INICIO</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	<a href="http://localhost:5000/"> SOBRE NOSOTROS</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	<a href="http://localhost:5000/"> CONTACTO</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
	<a href="http://localhost:5000/"> AYUDA</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

	
</div>
</body>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		background-color: black;
		width: 200;
	}
	
	body {
		text-align: center;
		padding: 1em;
		max-width: 1200px;
		margin: 0 auto;
		background-color: black;
		
	}
	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
	:global(h1)
	{
		color: #750c0c;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}
	:global(h2)
	{
		vertical-align:middle;
		color: #750c0c;
		text-transform: uppercase;
		font-size: 2em;
		font-weight: 10;
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
		font-size: 18px; 
		border: brown;
		background-image: -moz-repeating-linear-gradient(black,rgb(65, 9, 9)); 
		color: rgb(255, 255, 255); 
		border-radius: 50px; 
	}
	input[type=text]:Click
	{
		text-align: center;
		font-size: 18px; 
		border: brown;
		background-image: -moz-repeating-linear-gradient(black,rgb(65, 9, 9)); 
		color: rgb(255, 255, 255); 
		border-radius: 20px; 
		
	}
	input:focus {  border-image: #000000; }
	input[type=image]{

	max-width: 60px;
	max-height: 60px;
	font-size: 17px;
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
	border: 5px solid rgb(65, 9, 9);
	border-radius: 50px;
	width: 740px;
	padding: 20px;
	margin: 10px;
	}
	#suscripcion
	{
		float: right;
	align-self: center;
	text-align: center;
	border: 5px solid rgb(65, 9, 9);
	border-radius: 50px;
	width: 250px;
	padding: 20px;
	margin: 10px;
	}
	#destacada
	{
		float: right;
	align-self: center;
	text-align: center;
	border: 5px solid rgb(65, 9, 9);
	border-radius: 50px;
	width: 250px;
	padding: 20px;
	margin: 10px;
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
	#footer
	{
		background-image: linear-gradient(rgb(65, 9, 9) 0%, rgb(158, 80, 80) 50%, rgb(54, 12, 12) 100%);
	float:left;
	align-self: center;
	text-align: center;
	
	border-radius: 50px;
	width: 90%;
	padding: 20px;
	margin: 10px;
	}


</style>
