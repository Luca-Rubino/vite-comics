<script>

export default{
    data() {
        return{
            
        }
    },
    props:{
        singleComic:{
            type: Object,
            required: true,
        }
    }
}

</script>

<template>
    <article>
        <img :src="singleComic.thumb" :alt="singleComic.series">
        <h4>
            {{ singleComic.series }}
        </h4>
    </article>
</template>

<style lang="scss" scoped>
    article{
        padding: 1rem;

        img{
            width: 100%;
            height: 8rem;
            object-fit: cover;
            object-position: top;
        }
        h4{
            color: white;
            font-size: 1rem;
        }
    }
</style>