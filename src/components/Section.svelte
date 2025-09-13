<script>
    import Button from "../ui/Button.svelte";

    export let image;
    export let title;
    export let description;
    export let buttonText;

    export let positionY; //start, center, end
    export let positionX; //start, center, end

    //justify-content prop
    switch(positionX){
        case "left":
            positionX = "flex-start";
            break;
        case "center":
            positionX = "center";
            break;
        case "right":
            positionX = "flex-end";
            break;
        default:
            positionX = "flex-start";
    };

    //align-items prop
    switch(positionY){
        case "top":
            positionY = "flex-start";
            break;
        case "center":
            positionY = "center";
            break;
        case "bottom":
            positionY = "flex-end";
            break;
        default:
            positionY = "center";
    };

</script>

<main style="display: flex; justify-content: {positionX}; align-items: {positionY}">
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

    main {
        position: relative;
        width: 100%;
        height: 100vh;
        /* display: flex;
        align-items: center;
        justify-content: flex-start; */
        padding-left: 4rem;
        overflow: hidden;
        }

    img {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;      /* <── fills the whole area */
        z-index: -1;
    }

    .content{
        height: 280px;
        max-width: 600px;
        padding: 170px 220px;
    }

    h2{
        margin: 0px;
        text-transform: uppercase;
        font-family: "D-DIN-Bold", sans-serif;
        font-weight: bold;
        color: #F0F0FA;
        font-size: 47px;

    }

    p{
        font-family: "D-DIN";
    }
</style>