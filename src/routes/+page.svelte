<script lang="ts">
	let currentYear = new Date().getFullYear();
</script>

<main class="rounded-xl bg-card-bg p-6 md:p-8">
	<section class="mb-8 text-center text-lg">
		<p>Welcome! This is a repository of my academic texts, all two of them!</p>
		<p>Take a look by clicking on the sections below.</p>
	</section>

	<nav class="my-8 grid grid-cols-1 gap-8 sm:grid-cols-2">
		<div
			class="flex w-full flex-col-reverse rounded-md bg-small-card-bg p-0 shadow-md transition-transform duration-300 ease-in-out hover:-translate-y-1 hover:shadow-lg md:flex-col"
		>
			<a href="/bachelor" class="">
				<h1 class="mt-0 p-8 text-2xl">Bachelor's Thesis</h1>
			</a>
		</div>
		<div
			class="flex w-full flex-col-reverse rounded-md bg-small-card-bg p-0 shadow-md transition-transform duration-300 ease-in-out hover:-translate-y-1 hover:shadow-lg md:flex-col"
		>
			<a href="/master" class="">
				<h1 class="mt-0 p-8 text-2xl">Master's Thesis</h1>
			</a>
		</div>
	</nav>

	<!-- <section class="mt-12 p-6 rounded-md border-l-4 border-[#667eea]">
				<h3 class="mt-0 text-[#667eea]">Random Academic Wisdom</h3>
				<ul class="list-none p-0">
					<li class="py-2 text-lg">☕ Research is 10% inspiration, 90% caffeine</li>
					<li class="py-2 text-lg">📚 Every great thesis starts with a single question</li>
					<li class="py-2 text-lg">💡 The best ideas often come at 3 AM</li>
					<li class="py-2 text-lg">🎓 Knowledge is the only treasure that increases when shared</li>
				</ul>
			</section> -->
</main>

<footer class="mt-8 py-4 text-center text-white opacity-90">
	<p>&copy; {currentYear} | Kkobari</p>
</footer>
