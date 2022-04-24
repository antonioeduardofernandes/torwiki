<script>
    import Quote from "./Quote.svelte";
</script>

<section class="descriptions">
    <h3>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Distinctio,
        fugit dolore, tempore quasi nam soluta consequuntur repellat nihil
        mollitia earum id recusandae! Sit reprehenderit aliquid non ex, vel
        neque dolorem.
    </h3>
    <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda
        quibusdam optio facere eum maiores provident cumque laborum soluta dicta
        earum tenetur suscipit ipsa consequuntur debitis mollitia ad placeat
        omnis vero quia architecto, necessitatibus, sequi maxime vel illo.
        Repellendus, ex delectus? Omnis, non. Veritatis dicta blanditiis
        voluptatibus at vero vel eligendi.
    </p>
    <Quote />

    <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda
        quibusdam optio facere eum maiores provident cumque laborum soluta dicta
        earum tenetur suscipit ipsa consequuntur debitis mollitia ad placeat
        omnis vero quia architecto, necessitatibus, sequi maxime vel illo.
        Repellendus, ex delectus? Omnis, non. Veritatis dicta blanditiis
        voluptatibus at vero vel eligendi.
    </p>

    <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda
        quibusdam optio facere eum maiores provident cumque laborum soluta dicta
        earum tenetur suscipit ipsa consequuntur debitis mollitia ad placeat
        omnis vero quia architecto, necessitatibus, sequi maxime vel illo.
        Repellendus, ex delectus? Omnis, non. Veritatis dicta blanditiis
        voluptatibus at vero vel eligendi.
    </p>
</section>

<style>
    .descriptions {
        padding: 2rem;
        display: flex;
        flex-flow: column;
        justify-content: center;
        row-gap: 3rem;
    }

    h3 {
        text-align: center;
    }

    p {
        font-family: "Roboto", sans-serif;
        font-size: 0.8rem;
        text-align: justify;
    }
</style>
