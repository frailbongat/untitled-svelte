<script lang="ts">
	import { dev } from '$app/environment';
	import { SiteFooter, SiteHeader, TailwindIndicator } from '$lib/components/index.js';
</script>

<SiteHeader />
<div class="flex-1">
	<slot />
</div>
<SiteFooter />
{#if dev}
	<TailwindIndicator />
{/if}
