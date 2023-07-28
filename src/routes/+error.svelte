<script lang="ts">
	import { page } from '$app/stores';
</script>

<div class="space-y-5 text-center py-28">
	<p class="text-6xl font-bold tracking-widest text-error">{$page.status}</p>
	<h1 class="font-bold tracking-wider text-8xl">{$page?.error?.message}</h1>
</div>
