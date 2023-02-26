<script>
	import '@skeletonlabs/skeleton/themes/theme-skeleton.css';
	import '@skeletonlabs/skeleton/styles/all.css';
	import '../app.postcss';
    import { AppShell, AppBar } from '@skeletonlabs/skeleton';
</script>


<AppShell slotSidebarLeft="bg-surface-500/5 w-56 p-4">
    <svelte:fragment slot="header">
    <AppBar gridColumns="grid-cols-3" slotDefault="place-self-center" slotTrail="place-content-end">
        <svelte:fragment slot="lead">(icon)</svelte:fragment>
        DDDDonuts
        <svelte:fragment slot="trail">(actions)</svelte:fragment>
    </AppBar>
	</svelte:fragment>
    <svelte:fragment slot="sidebarLeft">
	<nav class="list-nav">
		<ul>
			<li><a href="/">Home</a></li>
			<li><a href="/about">About</a></li>
		</ul>
	</nav>
    </svelte:fragment>
    <slot />
    <svelte:fragment slot="footer">Footer</svelte:fragment>
</AppShell>
