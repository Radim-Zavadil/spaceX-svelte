<script>
    let items = ["VEHICLES", "LAUNCHES", "HUMAN SPACEFLIGHT", "RIDESHARE", "STARLINK", "STARSHIELD", "COMPANY", "SHOP"];
</script>

<main>
    <div class="navigationGroup">
        <img src="/img/spaceX-logo.png" alt="spaceX logo">
        <ul>
            {#each items as item}
                <li>{item}</li>
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
        font-size: 0.82em;
        font-weight: 700;
        letter-spacing: 0.09em;
        font-family: "D-DIN";
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