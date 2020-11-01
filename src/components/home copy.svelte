<script>
	let src = 'pngwing.com.png'
	let enable = true;
	let y;

	function typewriter(node, { speed = 50 }) {
		const valid = (
			node.childNodes.length === 1 &&
			node.childNodes[0].nodeType === Node.TEXT_NODE
		);

		if (!valid) {
			throw new Error(`This transition only works on elements with a single text node child`);
		}

		const text = node.textContent;
		const duration = text.length * speed;

		return {
			duration,
			tick: t => {
				const i = ~~(text.length * t);
				node.textContent = text.slice(0, i);
			}
		};
	}


</script>

<main>
	<div class="mydiv">
		<img {src} alt="logo" width='50%'/>
	

	<div class="scrollTrans">
		<span style="opacity: {1 - Math.max(0, y / 500)}">
			{#if y>=0}
			<h1 in:typewriter>Hello, I'm Adam!
			Student, (designer) and future 
			developer </h1>
			{/if}
		</span>
	</div>
</div>

</main>


<svelte:window bind:scrollY={y}/>



<style>

	.mydiv {
		position:relative
	}

	.mydiv img {
		position:absolute;
    top:0;
    left:40%;
	}


	main {

		padding: 1em;
		max-width: 140px;
		margin: 0 auto;
		margin-bottom: 10rem;
		padding-right:25%;
	}

	h1 {
		background: url(/home/adam/Projects/portf/portfolio/public/pngwing.com.png) no-repeat center 100px;
		background-size: 400px auto;
		position: fixed;
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


	span {
		display: block;
		font-size: 1em;
		text-transform: uppercase;
		will-change: transform, opacity;
	}
	
</style>