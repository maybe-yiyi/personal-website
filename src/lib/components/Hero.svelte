<script>
	const infostring = 'Information Systems @ CMU\nClass of 2029';
	let information = $state('');

	let done = $state(false);
	let i = 0;
	const interval = setInterval(() => {
		information += infostring[i];
		i++;
		if (i >= infostring.length) {
			clearInterval(interval);
			done = true;
		}
	}, 50);
</script>

<section id="hero">
	<div id="hero-content">
		<p id="hello">Hello, I'm</p>
		<h1 id="name">Yiyoung<br />Liu</h1>
		<p id="info">
			<span id="info-placeholder" aria-hidden="true">{infostring}</span>
			<span id="info-text">{information}<span class="cursor" class:done>_</span></span>
		</p>
	</div>
</section>

<style>
	#hero {
		flex: 1;
		display: flex;
		align-items: center;
		padding: 1.5rem 0.5rem;
	}

	#hero-content {
		max-width: 48rem;
		width: 100%;
		margin-inline: auto;
	}

	#hello {
		text-transform: uppercase;
		color: var(--color-blue);

		margin-botton: 1rem;
	}

	#info {
		position: relative;
		white-space: pre-line;
	}

	#info-placeholder {
		visibility: hidden;
		user-select: none;
	}

	#info-text {
		position: absolute;
		top: 0;
		left: 0;
	}

	.cursor.done {
		animation: blink 1s step-start infinite;
	}

	@keyframes blink {
		0%,
		100% {
			opacity: 1;
		}
		50% {
			opacity: 0;
		}
	}

	#name {
		font-family: sans-serif;
		font-size: 8rem;
		font-weight: bold;
		letter-spacing: -0.1rem;

		margin-top: 0rem;
		margin-bottom: 1rem;
	}
</style>
