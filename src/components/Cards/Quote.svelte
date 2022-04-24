<section>
    <div class="quote">
        <div class="top">
            <div class="img_container">
                <img
                    src="https://i0.wp.com/lamcdn.net/wonderzine.com/post_image-image/1X40UaX1AIIWWxYGBx386w-article.jpg"
                    alt="galadriel"
                />
            </div>
            <div class="play_button">
                <img src="assets/play_triangle.png" alt="" />
            </div>
        </div>
    </div>
    <div class="quote_text">
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Et quidem
        debitis accusantium magnam ut animi! Eaque assumenda libero rerum quis."
    </div>
</section>

<style>
    section {
        display: flex;
        flex-flow: column;
        align-items: center;
        row-gap: 3rem;
    }

    .top {
        position: relative;
    }

    .img_container {
        width: 80px;
        height: 80px;
        border-radius: 50%;
        overflow: hidden;
        align-self: center;
        position: relative;
    }

    .img_container img {
        height: 100%;
        width: 100%;
        object-fit: cover;
    }

    .play_button {
        width: 36px;
        height: 36px;
        position: absolute;
        bottom: -28px;
        left: -24px;
        border: 1px solid white;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .play_button img {
        height: 10px;
        width: 10px;
        transform: rotate(90deg);
    }

    .quote_text {
        font-size: 0.8rem;
        font-style: italic;
        text-align: center;
        opacity: 0.4;
    }
</style>
