<script>
    import TopContent from "./TopContent.svelte";
    import Descriptions from "./Descriptions.svelte";
    import Illustrations from "./Illustrations.svelte";
</script>

<div class="container">
    <TopContent />
    <Descriptions />
    <Illustrations />
</div>

<style>
    .container {
        display: flex;
        flex-flow: column;
    }
</style>
