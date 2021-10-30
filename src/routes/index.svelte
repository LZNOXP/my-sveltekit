<script lang="ts">
	import { goto } from '$app/navigation';

	let value: string = '';
	console.log('hello');
</script>

<svelte:head>
	<title>Template</title>
</svelte:head>

<h1 class="bg-green-500">Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<input class="border-green-800 border" type="text" bind:value />
<button class="border border-blue-500 p-4" on:click={() => goto(`/hello/${value}`)}>
	Say hello
</button>
