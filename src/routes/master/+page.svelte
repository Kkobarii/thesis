<script lang="ts">
	import { onMount } from 'svelte';
	import { base } from '$app/paths';

	let pdfUrl = `${base}/master.pdf`;
	let pdfExists: boolean = false;
	let checking: boolean = true;

	onMount(async () => {
		try {
			const res = await fetch(pdfUrl, { method: 'HEAD' });
			pdfExists = res.ok;
		} catch (_) {
			pdfExists = false;
		} finally {
			checking = false;
		}
	});
</script>

<header class="mb-8 text-white md:mb-12">
	<h1 class="mb-4 text-2xl md:mb-6 md:text-4xl">Master's Thesis</h1>
	<nav>
		<a href="/" class="text-grey no-underline hover:text-white">← Back to Home</a>
	</nav>
</header>

<main class="min-h-[400px] rounded-xl bg-card-bg p-6 md:p-8">
	{#if checking}
		<p>Checking for PDF...</p>
	{:else if pdfExists}
		<object
			data={pdfUrl}
			type="application/pdf"
			class="h-[600px] w-full md:h-[800px]"
			aria-label="Master's Thesis PDF Viewer"
		>
			<p>
				Your browser does not support PDFs.
				<a href={pdfUrl} class="text-blue-500 underline">Download the PDF</a> to view it.
			</p>
		</object>
	{:else}
		<div>
			<p>The PDF for the Master's thesis was not found.</p>
		</div>
	{/if}
</main>
