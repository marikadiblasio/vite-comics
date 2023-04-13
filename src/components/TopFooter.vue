<template>
    <footer>
       <div class="container h-100 d-flex justify-content-between">
        <div class="text-white h-100 w-50 gy-4 d-flex flex-column flex-wrap">
            <ul v-for="(link, index) in links" :key="index" class="py-2 list-unstyled">
                <li class="fw-bold pb-1 fs-5">{{ link.title }} </li>
                <li v-for="topic in link.topics">{{ topic }}</li>
            </ul>
        </div>
        <div class="w-35"><img src="../assets/img/dc-logo-bg.png" alt="logo"></div>
       </div> 
    </footer>
</template>

<script>
    export default {
        name: 'TopFooter',
        data(){
            return{
               links: [
                {
                    title: 'DC COMICS',
                    topics: [
                        'Characters',
                        'Comics',
                        'Movies',
                        'TV',
                        'Games',
                        'Video',
                        'News'
                    ]
                },
                {
                    title: 'SHOP',
                    topics: [
                        'Shop DC',
                        'Shop DC Collectibles'
                    ]
                },
                {
                    title: 'DC',
                    topics: [
                        'Term Of Use',
                        'Privacy policy (New)',
                        'Ad Choices',
                        'Advertising',
                        'Jobs',
                        'Subscriptions',
                        'Talent Workshop',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Helps',
                        'Contact Us'
                    ]
                },
                {
                    title: 'SITES',
                    topics: [
                        'DC',
                        'MAD Magazines',
                        'DC Kids',
                        'DC Universe',
                        'DC Power Visa'
                    ]
                }
               ] 
            }
        }
    }
</script>

<style lang="scss" scoped>
    footer {
        background-image: url('../assets/img/footer-bg.jpg');
        height: 350px;
        overflow: hidden;
    }
    .w35{
        width: 35%;
    }
    img {
        object-position: center -50px;
        width: 100%;
    }
</style>