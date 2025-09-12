<script>
    import { ArrowRight } from "lucide-svelte";

    export let buttonText;
</script>

<main>
    <p>{buttonText}</p>
    <ArrowRight class="arrow"/>
</main>

<style>
    main{
        display: flex;
        justify-content: center;
        align-items: center;
        height: 50px;
        width: 70px;
        background-color: rgba(10, 10, 10, 0.517);
        padding: 0px 20px;
        border: 1px solid rgba(240, 240, 250, 0.35);
        border-radius: 5px;
        cursor: pointer;
        margin-top: 30px;
    }

    p{
        color: #f0f0fa;
        text-transform: uppercase;
        font-family: "D-DIN";
        margin-right: 5px;
        font-size: 0.75em;
    }

    .arrow{
        width: 10px;
        height: 10px;
        color: #f0f0fa;
    }

    main:hover {
        background-color: rgba(255, 255, 255, 0.517);
        transition-duration: 0.5s;
        transition-timing-function: cubic-bezier(0.19, 1, 0.22, 1);
    }

    main:hover p {
        color: #000;
    }

    main:hover .arrow{
        color: #000;
    }
</style>