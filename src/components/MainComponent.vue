<template>
    <div class="hero d-flex justify-content-center align-items-center">
        <div class="container fw-bold text-white">
         -- > Content goes here &lt; -- 
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MainComponent',
    }
</script>

<style lang="scss" scoped>
    .hero {
        background-image: url('../assets/img/jumbotron.jpg');
        height: 10vh;
        position: relative;
        z-index: 2;
        // filter: grayscale(1);
        // filter: brightness(.1);
    }
    .hero::after{
        content: '';
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        background-color: rgba(0,0,0,0.8);
        z-index: 1;
    }
    .hero  span{
            color: white;  
            filter: brightness(120%);
            z-index: 10;
         }
</style>