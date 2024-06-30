<script lang="ts">
	import { ModeWatcher } from 'mode-watcher';
	import '../app.css';
</script>

<ModeWatcher />
<div class="relative flex min-h-screen flex-col bg-background" id="page" data-vaul-drawer-wrapper>
	<slot />
</div>
