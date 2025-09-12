<script>
    import Button from "../ui/Button.svelte";

    export let image;
    export let title;
    export let description;
    export let buttonText;

    export let position;
</script>

<main>
    <img src={image} alt="">
    <div class="content">
        
        <div>
            <h2>{title}</h2>
            <p>{description}</p>
            <Button buttonText={buttonText} />
        </div>
    </div>
    
</main>

<style>

    main{
        position: relative;
        width: 100%;
        height: 100vh;
        display: flex;
        align-items: center;
        justify-content: flex-start;
        padding-left: 4rem;
    }

    .content{
        height: 280px;
        max-width: 600px;
    }

    img{
        position: absolute;
        width: 100vw;
        height: 100vh;
        z-index: -1;
        object-fit: contain;   /* keeps proportions, no crop */
        background: #000;
    }

    h2{
        margin: 0px;
        text-transform: uppercase;
        font-family: "D-DIN";
        font-weight: bold;
        font-size: 47px;
        letter-spacing: 2px;

    }

    p{
        font-family: "D-DIN";
    }
</style>