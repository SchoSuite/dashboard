<script>
    import Nav from "$lib/nav.svelte";
    import SideBar from "$lib/side_bar.svelte";
</script>

<SideBar />
<Nav />

<div class="wrapper">
    <slot></slot>
</div>

<style>
    .wrapper {
        display: inline-block;
    }
</style>
