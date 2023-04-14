<template>
    <div class="wrapper ">
        <div class="hero position-relative">
            <img src="../assets/img/jumbotron.jpg" alt="hero">
            <button class="text-uppercase fw-bold fs-5 btn btn-primary rounded-0">Current Series</button>
        </div>
        <div class="bg-black">
            <div class="container  h-100 text-white">
                <div class="row">
                    <CardComponent :image="card.thumb" :title="card.series" v-for="card in cards"/>
                </div>
                <button class="text-uppercase mx-auto d-block btn btn-primary rounded-0">Load More</button>
            </div>
        </div>
    </div>
</template>

<script>
    import {cards} from '../data/data';
    import CardComponent from './CardComponent.vue';
    export default {
        name: 'MainComponent',
        components: {
            CardComponent
        },
        data(){
            return{
                cards: [...cards]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .wrapper{
        height: calc(100vh - (300px + 90px + 55px + 90px));
    }
    .hero {
        width: 100%;
        height: 300px;
        img {
            display: block;
            width: 100%;
            height: 300px;
            object-fit: cover;
            object-position: top;
        }
    }
    button.fs-5{
        // transform: translate(0, -50%);
        position: absolute;
        bottom: -5%;
        left: 3%;
        z-index: 100;
    }
    .bg-black{
        height: calc(100% - 300px);
        overflow-y: auto;
    }
</style>