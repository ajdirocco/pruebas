<script>
	// Follow @kevmodrome on Twitter for more fun Svelte things: https://twitter.com/kevmodrome
    import notifications from '../stores/notifications.js'
	import Toast from '$lib/Toast.svelte'
	
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<button on:click={() => notifications.info('Wait a INFO...', 100)}>
	info!
</button>
<button on:click={() => notifications.warning('Wait a moment...', 5000)}>
	Warn!
</button>
<button on:click={() => notifications.success('You did it!', 3000)}>
	Succeed!
</button>
<button on:click={() => notifications.danger('STOP NOW!', 500)}>
	Danger!
</button>
<button on:click={() => notifications.default('default', 1000)}>
	Default!
</button>
<Toast />
