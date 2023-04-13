<template>
    <div class="hero d-flex justify-content-center align-items-center">
        <div class="container fw-bold text-white">
        <span> -- > Content goes here &lt; -- </span>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MainComponent'
    }
</script>

<style lang="scss" scoped>
    .hero {
        background-image: url('../assets/img/jumbotron.jpg');
        padding-top: 3rem;
        padding-bottom: 3rem;
        position: relative;
        z-index: -2;
         span {
             z-index: 3;
         }
    }
    .hero::after{
        content: '';
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        background-color: rgba(0,0,0,0.95);
        z-index: -1;
    }
</style>