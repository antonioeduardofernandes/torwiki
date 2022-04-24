<script>
    import { gsap, Expo } from "gsap";

    const closeMenu = () => {
        gsap.to(".overlay_menu", {
            duration: 1,
            left: "-200%",
            ease: Expo.easeInOut,
        });
    };
</script>

<div class="overlay_menu">
    <div class="button close_button" on:click={closeMenu}>
        <svg viewBox="0 0 24 24"
            ><path
                d="M23.954 21.03l-9.184-9.095 9.092-9.174-2.832-2.807-9.09 9.179-9.176-9.088-2.81 2.81 9.186 9.105-9.095 9.184 2.81 2.81 9.112-9.192 9.18 9.1z"
            /></svg
        >
    </div>
    <div class="links">
        <div>Índice</div>
        <div class="sublinks">
            <div>PERSONAGENS</div>
            <div>LOCAIS</div>
            <div>EVENTOS</div>
            <div>BESTIÁRIO</div>
            <div>ITENS</div>
        </div>
    </div>
</div>

<style>
        .overlay_menu {
        position: fixed;
        width: 100vw;
        height: 100%;
        background-color: white;
        z-index: 99;
        display: flex;
        flex-flow: column;
        padding: 1rem;
        left: -200%;
    }

    .button {
        --button-size: 2.3rem;
        width: var(--button-size);
        height: var(--button-size);
        border: 0.2px solid rgba(255, 255, 255, 1);
        border-radius: 50%;
        background-color: transparent;
        display: flex;
        align-items: center;
        justify-content: center;
        opacity: 0.7;
        z-index: 2;
    }


    .close_button {
        border-color: rgba(0, 0, 0, 0.6);
        opacity: 0.6;
    }
    .close_button svg {
        --close_button-size: 9px;
        width: var(--close_button-size);
        height: var(--close_button-size);
    }
    .links {
        margin-top: 3rem;
        display: flex;
        flex-flow: column;
        row-gap: 3rem;
        margin-left: 2rem;
        font-size: 0.9rem;
    }

    .sublinks {
        display: flex;
        flex-flow: column;
        row-gap: 2rem;
        color: gray;
    }
</style>
