<script>
    import TopContent from "./TopContent.svelte";
    import Descriptions from "./Descriptions.svelte";
    import Gallery from "./Gallery.svelte";
</script>

<div class="container">
    <TopContent />
    <Descriptions />
    <Gallery />
    <img class="bg_rocks" src="assets/rocks_bg.png" alt="">
</div>

<style>
    .container {
        display: flex;
        flex-flow: column;
        row-gap: 4rem;
    }

    .bg_rocks {
        position: fixed;
        opacity: .1;
        height: 100%;
        width: 100%;
        top: 0;
        left: 0;
    }
</style>
