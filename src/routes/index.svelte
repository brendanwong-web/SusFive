<script>
	import successkid from 'images/successkid.jpg';
	import Button from '../components/Button.svelte';
</script>

<style lang="scss" global>
	 @import "./style/theme.scss";

	.container-main {
		padding: 3rem 15px 1rem;
		display: flex;
		flex-direction: column;
		justify-content: space-between;

		@media screen and (min-width: 560px) {
		padding: 4rem 15vw;
		display: flex;
		
		flex-direction: row;
		justify-content: space-between;
	}
	}

	.left {
		flex: 1 1 100%;
		@media screen and (min-width: 560px) {
			flex: 1 1 50%;
		}
		img {
			width: 100%;
			height: auto;
		}
	}

	.right {
		padding: 1rem;
		flex: 1 1 100%;
		text-align: left;

		@media screen and (min-width: 560px) {
			padding: 1rem 0;
		}

		& button:last-child {
			display: block;
			margin: 0 auto; 
			@media screen and (min-width: 560px) {
				margin: 0;
			}
		}

		@media screen and (min-width: 560px) {
			padding: 5rem 8rem 0 0;
			flex: 1 1 50%;
			text-align: left;
		}

		

		h2 {
			color: $blue-1;
			font-weight: 300;
			font-size: 1.1rem;
		}

		h1 {
			color: $green-2;
			font-weight: 500;
			font-size: 2rem;
		}

		p{
			color: $blue-3;
		}
	}
</style>

<svelte:head>
	<title>Sapper project template</title>
</svelte:head>

<div class="container-main">
	<div class="left">
		<img src="landing-apge.png" alt="landing page image">
	</div>
	<div class="right">
		<h2>
			SusFive was created with one goal in mind: 
		</h2>
		<h1>
			To rid the world of pollution
		</h1>
		<p>
			Creating a better and more sustainable Earth for you .
		</p>
		<p>
			
Our plan is to use carbon eating bacteria to clean the air.	
		</p>
		<Button link="contact">Contact us</Button>
	</div>
</div>