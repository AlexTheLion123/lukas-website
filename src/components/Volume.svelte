<script>
    let a = 40;
</script>

<label class="volume-container">
    <input class="volume-num" type=number bind:value={a} min=0 max=100>
	<input class="slider" type=range bind:value={a} min=0 max=100>
</label>

<style>
    input[type="number"] {
        display: none;
    }

    .volume-container {
        transform: rotate(-90deg);
        position: absolute;
        width: 30%;
        top: 120px;
    }
    .slider {
        width: 100%;
    }
    .volume-num {
        transform: rotate(90deg)
    }
</style>