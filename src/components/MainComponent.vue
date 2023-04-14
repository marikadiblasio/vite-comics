<template>
    <div class="wrapper">
        <div class="hero">
            <img src="../assets/img/jumbotron.jpg" alt="hero">
        </div>
        <div class="bg-black h-100">
            <div class="container text-white">
                <button class="text-uppercase fw-bold fs-5 btn btn-primary rounded-0">Current Series</button>
                <div class="row">
                    <CardComponent />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import CardComponent from './CardComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
            CardComponent
        }
    }
</script>

<style lang="scss" scoped>
    .wrapper{
        height: calc(100vh - (300px + 90px + 55px + 90px));
    }
    .hero {
        width: 100%;
        height: 350px;
        img {
            display: block;
            width: 100%;
            height: 350px;
            object-fit: cover;
            object-position: top;
        }
    }
    button.fs-5{
        transform: translate(0, -50%);
    }
</style>