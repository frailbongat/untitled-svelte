<script lang="ts">
	import { ModeWatcher } from 'mode-watcher';
	import { SiteHeader } from '$lib/components/index.js';
	import '../app.css';
</script>

<ModeWatcher />
<SiteHeader />
<slot></slot>
