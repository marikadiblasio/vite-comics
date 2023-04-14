<template>
    <div class="col-12 col-md-4 col-lg-2 text-center">
            <img :src="image" :alt="title">
            <div class="text-uppercase small py-2">
                {{ title }}
            </div>
    </div>
</template>

<script>
    export default {
        name: 'CardComponent',
        props: ['image', 'title']
    }
</script>

<style lang="scss" scoped>
    img{
        width: 10rem;
        height: 10rem;
        text-align: center;
    }
</style>