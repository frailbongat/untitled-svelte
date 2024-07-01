<script lang="ts">
	import { ModeWatcher } from 'mode-watcher';
	import '../styles/globals.css';
	import { updateTheme } from '$lib/utils.js';
	import { config } from '$lib/stores/index.js';
	import { page } from '$app/stores';

	$: updateTheme($config.theme, $page.url.pathname);
</script>

<ModeWatcher />
<div class="relative flex min-h-screen flex-col bg-background" id="page" data-vaul-drawer-wrapper>
	<slot />
</div>
