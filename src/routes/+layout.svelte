<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<header
	class="h-0.125 flex flex-row items-center gap-6 bg-primary p-4 font-navbar text-navbar text-accent"
>
	<a href="/">home</a>
	<a href="/upload">upload books</a>
</header>

<main
	class="flex min-h-screen flex-col items-center bg-background font-normal text-normal text-secondary"
>
	{@render children()}
</main>
