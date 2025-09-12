<script>
    export let buttonText;
</script>

<main>
    <p>{buttonText}</p>

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
        color: #fff;
        text-transform: uppercase;
        font-size: 0.85em;
    }
</style>