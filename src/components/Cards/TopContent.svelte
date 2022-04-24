<section>
    <div class="main_img">
        <!-- <img
            src="https://i0.wp.com/lamcdn.net/wonderzine.com/post_image-image/1X40UaX1AIIWWxYGBx386w-article.jpg"
            alt="galadriel"
        /> -->
    </div>
    <div class="name">
        <h1>title</h1>
        <div class="scroll_indicator">Role para baixo</div>
    </div>
</section>

<style>

    .main_img {
        position: absolute;
        width: auto;
        height: 100vh;
        opacity: 0.4;
    }

    .main_img img {
        width: 100%;
        height: 100vh;
        object-fit: cover;
        object-position: center;
        overflow: hidden;
    }
    .name {
        height: 100vh;
        display: flex;
        flex-flow: column;
        row-gap: 3rem;
        justify-content: flex-end;
        text-align: center;
    }

    h1 {
        text-transform: uppercase;
        font-size: 1.4rem;
    }

    .scroll_indicator {
        opacity: 0.4;
        margin-bottom: 3rem;
    }
</style>
