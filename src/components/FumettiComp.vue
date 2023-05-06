<script>
export default {
    name: "FumettiComp",
    props: ['Fumetti'],
}
</script>

<template>
    <div class="fumetto">
        <img :src="Fumetti.thumb" alt="">
        <h4 class="white">{{ Fumetti.series }}</h4>
    </div>
</template>

<style lang="scss" scoped>
.fumetto {
    width: calc(100% / 6 - 10px);

    img {
        width: 100%;
        margin-bottom: 20px;
    }

}
</style>