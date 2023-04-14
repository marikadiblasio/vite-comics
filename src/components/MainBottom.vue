<template>
    <div class="bg-primary">
        <div class="container">
            <div class="row">
                <div v-for="link in mainLinks" class="col py-md-3 py-0 pe-3 d-flex align-items-center">
                    <div class="rem-3 pe-2"><img class="img-fluid" :src="link.image" alt="digital"></div>
                    <div>
                        <a href="#"><h6 class="text-uppercase text-white">{{ link.text }}</h6></a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MainBottom',
        data(){
            return{
                mainLinks: [
                    {
                        image: '/public-img/buy-comics-digital-comics.png',
                        text: 'digital comics'
                    },
                    {
                        image: '/public-img/buy-comics-merchandise.png',
                        text: 'dc merchandise'
                    },
                    {
                        image: '/public-img/buy-comics-subscriptions.png',
                        text: 'subscription'
                    },
                    {
                        image: '/public-img/buy-comics-shop-locator.png',
                        text: 'comic shop locator'
                    },
                    {
                        image: '/public-img/buy-dc-power-visa.svg',
                        text: 'dc power visa'
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .rem-3{
        width: 3rem;
        cursor: pointer;
    }
    // @media screen and (max-width: 992px) {
    //     a {
    //         display: none;
    //     }
    // }
</style>