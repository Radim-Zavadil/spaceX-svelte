<script>
    let items = ["careers", "updates", "privacy policy", "suppliers"];
</script>

<main>
    <div class="content">
        <div>
            <img src="/img/x-logo.svg" alt="X" class="twitter">
        </div>
        <div class="links">
            {#each items as item}
                <p class="text">{item}</p>
            {/each}
        </div>
        <p class="text">@2025 spaceX</p>
    </div>
    
</main>

<style>
    main{
        height: 50px;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        box-shadow: 0px -27px 17px #000;
    }

    .content{
        width: 100%;
        margin: 12px 60px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .links{
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .text{
        font-family: "D-DIN";
        font-size: 12px;
        color: #F0F0FA;
        text-transform: uppercase;
        padding: 17px;
        cursor: pointer;
    }

    .text:hover {
        opacity: 0.5;
        transition-duration: 0.7s;
        transition-timing-function: cubic-bezier(0.075, 0.82, 0.165, 1);
    }

    .twitter{
        width: 17px;
        height: 17px;
        cursor: pointer;
    }

    .twitter:hover {
        opacity: 0.5;
        transition-duration: 0.7s;
        transition-timing-function: cubic-bezier(0.075, 0.82, 0.165, 1);
    }

</style>