<script>
    let items = ["VEHICLES", "LAUNCHES", "HUMAN SPACEFLIGHT", "RIDESHARE", "STARLINK", "STARSHIELD", "COMPANY", "SHOP"];
</script>

<main>
    <div class="navigationGroup">
        <img src="/img/spaceX-logo.png" alt="spaceX logo">
        <ul>
            {#each items as item}
                <li><p>{item}</p></li>
            {/each}
        </ul>
    </div>
    
    <div class="timer">
        <p>Upcoming launches</p>
    </div>
</main>

<style>

    main{
        position: absolute;
        width: 100%; /*justify-content doesn't work if the width is not set*/
        top: 0;
        z-index: 100;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 47px;
    }

    .navigationGroup{
        display: flex;
        justify-content: center;
        align-items: center;
    }


    ul{
        display: flex;
        justify-content: center;
        align-items: center;
        list-style-type: none;
    }

    li{
        padding: 10px;
        margin: 10px;
    }

    li p{
        font-size: 0.82em;
        font-weight: 700;
        letter-spacing: 0.09em;
        font-family: "D-DIN";
        color: rgba(240,240,250, 0.7);
        text-shadow: 0 0 2px #F0F0FA70;
        cursor: pointer;
    }

    li p:hover{
        color: rgb(240,240,250);
        transition-duration: 0.7;
        transition-timing-function: cubic-bezier(0.175, 0.885, 0.32, 1.275);
    }



    img{
        width: 200px;
        
    }

    .timer{
        padding: 2px 17px;
        border: 1px solid rgba(142, 142, 142, 0.25);
        border-radius: 4px;
    }

    .timer p{
        text-transform: uppercase;
        font-family: "D-DIN";
        font-size: 0.72em;
        font-weight: 400;
        margin-right: 70px;
        letter-spacing: 1;
    }
</style>