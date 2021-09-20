<script>
    import Play from "./Play.svelte"
</script>

<div class="button-container">
        <Play on:click/>
</div>


<style>
    .button-container {
        bottom: 55px;
        right: 20px;
    }
    .play {
        position: absolute;
        z-index: 2;

        box-sizing: border-box;
        width: 74px;
        height: 74px;
        border-width: 37px 0px 37px 74px;
        border-color: transparent transparent transparent #202020;
    }
    
</style>