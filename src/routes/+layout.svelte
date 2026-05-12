<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<header
	class="h-0.125 hover: flex flex-row items-center gap-6 bg-primary p-4 font-navbar text-navbar text-accent"
>
	<a class="hover:underline" href="/">home</a>
	<a class="hover:underline" href="/login">log in</a>
	<a class="hover:underline" href="/upload">upload books</a>
</header>

<main
	class="flex min-h-screen flex-col items-center bg-background font-normal text-normal text-secondary"
>
	{@render children()}
</main>

<footer class="h-0.05 flex items-center bg-background font-normal text-normal text-secondary">
	<p>
		Contribute and see the code on our <a
			class="text-input hover:underline"
			href="https://github.com/alstocras/LibraryApp">GitHub</a
		>.
	</p>
</footer>
