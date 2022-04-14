<script>
    import TopContent from "./TopContent.svelte";
    import Descriptions from "./Descriptions.svelte";
    import BottomContent from "./BottomContent.svelte";
    import Illustrations from "./Illustrations.svelte";
</script>

<div class="container">
    <TopContent />
    <Descriptions />
    <BottomContent />
    <Illustrations />  
</div>

<style>
    .container {
        display: flex;
        flex-flow: column;
    }
    /* section {
        display: flex;
        flex-flow: column;
        height: 100vh;
        position: relative;
    } */

    
</style>
