<script lang="ts">
	import { username } from '$lib/store.svelte';
</script>

<h1 class="text-3xl">Log in</h1>

<br /><br />

<label for="name">Username</label>
<input
	type="text"
	placeholder="username"
	id="name"
	class="
		w-full
		max-w-md
		rounded-lg
		border-2
		border-primary/20
		bg-input
    p-3
		text-accent
		transition-all
		outline-none
		focus:border-primary
	"
	bind:value={username.name}
/>
<br />
<p>Hello, {username.name}.</p>
