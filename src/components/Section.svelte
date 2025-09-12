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
    <div>
        <h1>{title}</h1>
        <p>{description}</p>
        <Button buttonText={buttonText} />
    </div>
</main>

<style>

</style>