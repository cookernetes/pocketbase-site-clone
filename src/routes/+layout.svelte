<script lang="ts">
	import '../app.postcss';
    import Navbar from "$components/global/Navbar.svelte";
    import CollectionsAside from "$components/CollectionsAside.svelte";
</script>

<div class="grid parent">
    <div class="flex">
        <Navbar />
        <CollectionsAside />
    </div>

    <slot />
</div>

<style>
    .parent {
        display: grid;
        grid-template-columns: auto 1fr;
        grid-template-rows: auto;
        grid-column-gap: 0;
        grid-row-gap: 0;
    }
</style>