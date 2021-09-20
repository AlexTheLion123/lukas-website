<script>
	import Disc from './components/Disc.svelte'
	import Buttons from './components/Buttons.svelte'
	import Volume from './components/Volume.svelte'
</script>
<h1>Awe </h1>


<div class="container">
	<Buttons on:click={disc.animateHandle}/>
	<Disc bind:this={disc}/>
	<Volume/>
</div>

<style> 
	.container {
        position: relative;
        margin: auto;
        background: #95c1b5ff;
        height: 500px;
        width: 600px;
        border-radius: 10px;

        display: grid;
        place-items: center;
        grid-template-rows: 1fr 1fr;
        grid-template-columns: 1fr 1fr;

    }
</style>


