<script>
	export let name;
</script>

<main>
	<h1>Hello, I'm {name}!<br> Student, (designer) and future <br>developer 
	</h1>
</main>

<style>

	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		margin-top: 20rem;
		margin-left: 30rem;
		line-height: 1 ;
		text-align: left;
		color: whitesmoke;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>