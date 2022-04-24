<script>
    import { onMount } from "svelte";
    import { gsap } from "gsap";
    import { ScrollTrigger } from "gsap/ScrollTrigger";
    import {Power1, Sine} from "gsap"
    gsap.registerPlugin(ScrollTrigger);

    onMount(()=>{
        gsap.from(".main_img", {duration:1, scale:1.1, opacity:0, ease:Power1})
        gsap.from(".title", {duration:2, opacity:0, letterSpacing:30, ease:Sine})
        gsap.from(".scroll_indicator", {duration:1, opacity:0, y:30, ease:Power1})
    })
</script>

<section>
    <div class="main_img">
        <img
            src="https://quintacapa.com.br/wp-content/uploads/2017/12/Gandalf-2.jpg"
            alt="character"
        />
    </div>
    <div class="name">
        <h1 class="title">gandalf</h1>
        <div class="scroll_indicator">Role para baixo</div>
    </div>
</section>

<style>
    .main_img {
        position: absolute;
        width: auto;
        height: 100vh;
        overflow: hidden;
        opacity: .4;
    }
    
    .main_img img {
        width: 100%;
        height: 100vh;
        object-fit: cover;
        object-position: center;
    }
    .name {
        height: 100vh;
        display: flex;
        flex-flow: column;
        row-gap: 3rem;
        justify-content: flex-end;
        text-align: center;
    }

    .title {
        letter-spacing: 10px;
        text-transform: uppercase;
        font-size: 1.8rem;
    }

    .scroll_indicator {
        opacity: 0.4;
        margin-bottom: 3rem;
    }
</style>
