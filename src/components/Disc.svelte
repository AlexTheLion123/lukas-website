<script>
    import { selected } from '../stores.js'

    const animateHandle = () {
        const handle = document.querySelector('.hand-holder');
        
    }
</script>

    
    <div class="disc-container">
        <div class="disc"></div>
        <div class="hand-container">
            <div class="hand-holder"></div>
            <img src="../images/diamond-hand.svg" alt="">
        </div>

        <div class="sub-container"></div>
        
    </div>
    

<style>
    
    .disc-container {
        grid-area: 2 / 1;
        position: relative;
        width: 100%;
        height: 100%; 
        display: grid;
        place-items: center;
        background: #dd5763ff;
        border-radius: 10px;
        box-shadow: 3px 3px 3px;

        left: 30px;
        bottom: 30px;
        overflow: hidden;
    }
    .disc {
        width: 5px;
        height: 5px;
        background: black;
        border-radius: 100%;
        box-shadow: 
            0 0 0 30px rgb(150, 0, 0),
            0 0 0 35px black,
            0 0 0 80px rgb(31, 31, 31),
            0 0 0 82px rgb(168, 168, 168);
        z-index: 1;
        position: relative;
        right: 20px;
    }
    .hand-container {
        position: absolute;
        height: 250px;
        width: 100px;
        background: #dd5763ff;
        
        display: flex;
        flex-direction: column;
        align-items: center;

        right: 0px;
        top: 5px;
    }
    .hand-holder {
        position: absolute;
        width: 30px;
        height: 30px;
        border-radius: 100%;
        background: #1a161aff;
        box-shadow: 
            0 0 0 10px #28252aff,
            0 0 10px 9px;

        top: 38px;
        right: 35px;
        z-index: 2;
    }
    img {
        position: absolute;
        z-index: 2;
        /* right: 30px;
        top: 20px; */
        height: 65%;
    }

    .sub-container {
        position: absolute;
        height: 40%;
        width: 100%;
        background: #3c3237ff;
        bottom: 0;
    }
</style>