<script>
	import Login from './lib/Login.svelte';
	import Messages from './lib/messages.svelte';
	import { currentUser } from './lib/pocketbase';
</script>

<h1>Chat App</h1>

<Login />

{#if $currentUser}
	<Messages />
{/if}

