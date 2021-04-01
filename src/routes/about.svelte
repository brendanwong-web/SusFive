<style lang="scss" global>
	@import "./style/theme.scss";

	

.container {
    padding: 2rem 13vw;

    img {
        width: 100%;
        height: auto;
    }
}

.about .container--flex {
	.left {
	}
	.right {
		
		padding-left:1rem;
	}

	
}
   
section {
	background-color: $green-2-lighter;
	border-radius: 20px;
	box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px,
	rgba(0, 0, 0, 0.35) 0px 5px 15px;
	margin-bottom: 2rem;

	.title {
		background-color: $green-2;
		border-top-left-radius: 20px;
		border-top-right-radius: 20px;
		padding: 1.5rem;
		

		h1 {
			margin: 0;
			font-weight: 400;
			color: white;
		}
	}

	.content {
		padding: 1.5rem;
		color: $blue-3;

		img {
			border-radius: 7px;
			-webkit-box-shadow: inset 2px 2px 1px 0px rgba(0,0,0,0.49);
			-moz-box-shadow: inset 2px 2px 1px 0px rgba(0,0,0,0.49);
			box-shadow: inset 2px 2px 1px 0px rgba(0,0,0,0.49);
			-webkit-box-shadow: inset 2px 2px 36px -7px rgba(0,0,0,0.19);
			-moz-box-shadow: inset 2px 2px 36px -7px rgba(0,0,0,0.19);
			box-shadow: inset 2px 2px 36px -7px rgba(0,0,0,0.19);
		}

		p {
			margin-top: 0;
		}
	}
}
</style>

<svelte:head>
	<title>About</title>
</svelte:head>

<div class="container about">
	<section>
		<div class="title">
			<h1>
				About BACPAIR
			</h1>
		</div>
		<div class="content">
			<div class="container--flex">
				<div class="left">
					<img src="bacpair.jpg" alt="bacpair">
				</div>
				<div class="right">
					<p>
						Converts SO2, NO, and CO2 which are undesirable gases into useful energy gas. This will help ensure the short-term reduction of greenhouse gas emissions and the long-term betterment of the environment.
					</p>
					<p>
				
						Offering industries useful energy gas such as H2S, N2, methane, and hydrogen gas, which can be utilized internally or sold to other companies. 
					</p>
		
				</div>
			</div>
		</div>
	</section>
	<section>
		<div class="title">
			<h1>
					Why you should have BACPAIR
				</h1>
		</div>
		<div class="content">
			<ul>
				<li>First of it’s kind</li>
				<li>Short term reduction of green house gases will equate to long term benefit to our society
				</li>
				<li>
					Formation of useful end products which are of commercial value, Hydrogen Sulfide Gas and Nitrogen Gas</li>
				<li>Reduces the amount of carbon tax for companies</li>
			</ul>
		</div>
	</section>
	
	
	
</div>