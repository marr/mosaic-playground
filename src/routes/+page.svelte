<!-- YOU CAN DELETE EVERYTHING IN THIS PAGE -->
<script>
	import { onMount } from 'svelte';
	import vg from '$lib/vg';

	/** @type {import('./$types').PageData} */
	export let data;

	onMount(() => {
		document.querySelector('#output')?.appendChild(vg);
	});
</script>

<div class="container h-full mx-auto flex justify-center items-center">
	<div class="space-y-5">
		<h1 class="h1">Stock Closing Prices</h1>
		<div id="output" class="text-primary-500" />
		<p>Start by exploring:</p>
		<ul>
			<li>
				<code class="code">/src/routes/+layout.svelte</code> - barebones layout, the CSS import order
				is critical!
			</li>
			<li>
				<code class="code">/src/app.postcss</code> - minimal css to make the page full screen, may not
				be relevant for your project
			</li>
			<li>
				<code class="code">/src/routes/+page.svelte</code> - this page, you can replace the contents
			</li>
		</ul>
	</div>
</div>
