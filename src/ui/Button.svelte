<script>
    import { ArrowRight } from "lucide-svelte";

    export let buttonText;
</script>

<main>
    <p>{buttonText}</p>
    <ArrowRight class="arrow" color="currentColor" strokeWidth={1.2} size={22}/>
</main>

<style>
    main{
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 50px;
        width: fit-content;
        background-color: rgba(10, 10, 10, 0.517);
        padding: 0px 20px;
        border: 1px solid rgba(240, 240, 250, 0.35);
        border-radius: 5px;
        cursor: pointer;
        margin-top: 30px;
        color: #F0F0FA;
    }

    p{
        /* color: #f0f0fa; */
        text-transform: uppercase;
        font-family: "D-DIN";
        margin-right: 5px;
        font-size: 0.75em;
    }

    main:hover {
        background-color: #F0F0FA;
        transition-duration: 0.5s;
        transition-timing-function: cubic-bezier(0.19, 1, 0.22, 1);
        color: #000;
    }

    /* main:hover p {
        color: #000;
    } */

    /* main:hover *{
        color: #000;
    } */

</style>