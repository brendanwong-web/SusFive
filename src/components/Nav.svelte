<script>
	export let segment;
</script>

<style lang="scss" global>
	 @import "./style/theme.scss";
	nav {
		font-weight: 300;
		padding: 10px 15vw;

		.container {
			display: flex;
			justify-content: space-between;
			padding: 0 0;
		}

		.logo {
			display: grid;
			place-items: center;

			img {
				width: 50px;
				height: auto;
			}
		}

		ul {
			margin: 0;
			padding: 0;
		}

		/* clearfix */
		ul::after {
			content: '';
			display: block;
			clear: both;
		}

		li {
			display: block;
			float: left;
			font-size: 1.5rem;
		}		
	}

	

	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: $blue-3;
		display: block;
		bottom: -1px;
	}

	a {
		text-decoration: none;
		padding: 0.5em 0.5em;
		display: block;
	}
</style>

<nav>
	<div class="container">
		<div class="logo">
			<img src="logo-512.png" alt="logo">
		</div>
		<ul>
			<li><a aria-current="{segment === undefined ? 'page' : undefined}" href=".">home</a></li>
			<li><a aria-current="{segment === 'about' ? 'page' : undefined}" href="about">about</a></li>
			<li><a aria-current="{segment === 'contact' ? 'page' : undefined}" href="contact">contact</a></li>
		</ul>
	</div>
	
</nav>
