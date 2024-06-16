<script>

</script>

<template>

<section class="d-flex">

<article class="d-flex">
    <button>sing-up now!</button>
</article>

<article class="d-flex">
    <h2>follow us</h2>
    <img src="/src/assets/img/footer-facebook.png">
    <img src="/src/assets/img/footer-twitter.png">
    <img src="/src/assets/img/footer-youtube.png">
    <img src="/src/assets/img/footer-pinterest.png">
    <img src="/src/assets/img/footer-periscope.png">
</article>

</section>

</template>

<style lang="scss" scoped>
section {
    background-color: #303030;
    width: 100%;
    justify-content: center;
    padding: 2rem 0;

    article {
        align-items: center;
        width: 50%;
    }

    article:first-child {
        padding-left: 19rem;
    }

    article:nth-child(2) {
        padding-left: 12.5rem;
    }

    button {
        border: 1px solid #008cff;
        background: transparent;
        padding: .8rem;
        color: white;
        text-transform: uppercase;
        font-weight: 900;
        font-family: Arial, Helvetica, sans-serif;
    }

    h2 {
        margin-right: 1.2rem;
        color: #0380f6;
        font-size: 1.2rem;
        text-transform: uppercase;
    }

    img {
        margin-right: 1rem;
    }
}
</style>