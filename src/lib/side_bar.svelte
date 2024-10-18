<script>
    import Shortcut from "$lib/shortcut.svelte";
</script>

<div id="main">
    <Shortcut text="jk" />
    <Shortcut text="jk" />
    <Shortcut text="jk" />
    <Shortcut text="jk" />
    <Shortcut text="jk" />
    <Shortcut text="jk" />
    <Shortcut text="jk" />
    <Shortcut text="jk" />
    <Shortcut text="jk" />
</div>

<style>
    @import "/theme.css";

    #main {
        background-color: var(--bg2);
        position: fixed;
        left: 0px;
        top: 0px;
        padding-top: 70px;
        padding-left: 5px;
        padding-right: 5px;
        height: 100%;
        border-left: 5px solid var(--blue);
        box-shadow: 0px 0px 5px var(--black);
    }
</style>
