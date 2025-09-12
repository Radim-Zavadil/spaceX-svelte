<script>
    let items = ["VEHICLES", "LAUNCHES", "HUMAN SPACEFLIGHT", "RIDESHARE", "STARLINK", "STARSHIELD", "COMPANY", "SHOP"];
</script>

<main>
    <div class="navigationGroup">
        <img src="../../public/img/spaceX-logo.png" alt="spaceX logo">
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
        display: flex;
        justify-content: space-around;
        align-items: center;
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

    img{
        width: 30px;
        height: 30px;
    }

    .timer{
        padding: 15px 30px;
        border: 2px solid rgba(255,255,255, 0.25);
        border-radius: 4px;
    }

    .timer p{
        text-transform: uppercase;
    }
</style>