<script lang="ts">
	let username: string = $state('');
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
		p-3
		text-input
		transition-all
		outline-none
		focus:border-primary
	"
	bind:value={username}
/>
<br />
<p>Hello, {username}.</p>
