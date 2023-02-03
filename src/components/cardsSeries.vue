<script>
export default{
    name: 'cardsSeries',
    props: {
        title: String,
        src: String,
    }
}
</script>

<template>
    <div>
        <div class="img-series">
            <img :src="src" :alt="title">
        </div>
        <p>{{ title }}</p>
    </div>
</template>

<style lang="scss" scoped>
.card{
    width: calc(100% / 6);
    padding: 10px;
    padding-bottom: 30px ;
}
.img-series{
    width: 100%;

    img{
        width: 100%;
        height: 180px;
        object-fit: cover;
        object-position: top;
    }
}
</style>