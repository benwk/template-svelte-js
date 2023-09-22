<script>
	import Button from '$lib/components/ui/button/button.svelte';
	import { Skeleton } from '$lib/components/ui/skeleton';
	import { Loader2 } from 'lucide-svelte';
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<Button>Get early access</Button>

<Button disabled>
	<Loader2 class="mr-2 h-4 w-4 animate-spin" />
	Wait a moment
</Button>

<Button>
	<Loader2 class="mr-2 h-4 w-4 animate-spin" />
	Get early access
</Button>

<br />

<div class="flex items-center space-x-4">
	<Skeleton class="h-12 w-12 rounded-full" />
	<div class="space-y-2">
		<Skeleton class="h-4 w-[250px]" />
		<Skeleton class="h-4 w-[200px]" />
	</div>
</div>
