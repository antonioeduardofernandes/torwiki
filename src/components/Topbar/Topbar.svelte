<script>
    import { onMount } from "svelte";
    import { gsap, Expo } from "gsap";
    import OverlayMenu from "./OverlayMenu.svelte";

    // let clickSound = new Audio("audio/buttonClick.mp3");
    const openMenu = () => {
        // clickSound.play();
        gsap.to(".overlay_menu", {
            duration: 1,
            left: 0,
            ease: Expo.easeInOut,
        });
    };
</script>

<OverlayMenu />

<div id="topbar">
    <!-- Left Content -->
    <div class="left_content">
        <div class="button mini">
            <svg viewBox="0 0 30 30" fill="none"
                ><path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M15 0C6.716 0 0 6.716 0 15c0 8.284 6.716 15 15 15 8.284 0 15-6.716 15-15 0-8.284-6.716-15-15-15zm-3.427 7.495l-.571.52V15.5l-.002.001V18l-.95-1.899-1.048.663v6.773L12.275 25l5.727-1.463v-4.968L16.716 17.5V7.852L14.466 5h-1.928v2.495h-.965z"
                    fill="#ffffff"
                /></svg
            >
        </div>
        <!-- Return Button -->
        <div class="button">
            <svg
                viewBox="0 0 24 24"
                class="return_icon"
                fill="#ffffff"
                style=" transform: rotate(180deg)"
                ><path
                    d="M21.883 12l-7.527 6.235.644.765 9-7.521-9-7.479-.645.764 7.529 6.236h-21.884v1h21.883z"
                /></svg
            >
        </div>
    </div>
    <!-- Menu button -->
    <div class="button menu_button" on:click={openMenu}>
        <div class="dot" />
        <div class="dot" />
        <div class="dot" />
    </div>
</div>

<style>
    #topbar {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 1rem;
        position: fixed;
        z-index: 98;
        top: 0;
        left: 0;
        right: 0;
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
    .mini {
        --button-size: 2rem;
        width: var(--button-size);
        height: var(--button-size);
        opacity: 0.2;
        border: none;
    }
    .left_content {
        display: flex;
        column-gap: 0.5rem;
        align-items: center;
    }
    .return_icon {
        --icon-size: 18px;
        width: var(--icon-size);
        height: var(--icon-size);
    }
    .menu_button {
        column-gap: 0.1rem;
    }
    .dot {
        --dot-size: 5px;
        width: var(--dot-size);
        height: var(--dot-size);
        border-radius: 50%;
        background-color: white;
    }
</style>
