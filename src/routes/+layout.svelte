<script lang="ts">
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="min-h-screen bg-page-bg text-white">
	<div class="mx-auto max-w-[1200px] p-8 pt-0 font-sans">
		<header class="mb-12 rounded-b-xl bg-card-bg py-8 text-center">
			<h1 class="mb-2 text-3xl md:text-5xl">Kkobari's Academic Writing</h1>
			<p class="text-lg text-grey">A collection of my theses</p>
		</header>

		{@render children()}
	</div>
</div>
