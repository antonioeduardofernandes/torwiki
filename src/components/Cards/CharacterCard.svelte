<script>
    import TopContent from "./TopContent.svelte";
    import Descriptions from "./Descriptions.svelte";
    import Gallery from "./Gallery.svelte";
</script>

<div class="container">
    <TopContent />
    <Descriptions />
    <Gallery />
</div>

<style>
    .container {
        display: flex;
        flex-flow: column;
        row-gap: 4rem;
    }
</style>
