<template>
    <header class="bg-white">
        <div class="container d-flex justify-content-between align-items-center">
            <div><img class="img-fluid" src="../assets/img/dc-logo.png" alt="Logo"></div>
            <nav>
                <ul class="d-flex flex-wrap align-items-center list-unstyled">
                    <li v-for="navLink in navLinks" class="pe-4"><a :href="navLink.ref">{{navLink.navTopic}}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data(){
            return{
                navLinks: [
                    {
                        ref: '#',
                        navTopic: 'character'
                    },
                    {
                        ref: '#',
                        navTopic: 'comics'
                    },
                    {
                        ref: '#',
                        navTopic: 'movies'
                    },
                    {
                        ref: '#',
                        navTopic: 'tv'
                    },
                    {
                        ref: '#',
                        navTopic: 'games'
                    },
                    {
                        ref: '#',
                        navTopic: 'collectibles'
                    },
                    {
                        ref: '#',
                        navTopic: 'videos'
                    },
                    {
                        ref: '#',
                        navTopic: 'fans'
                    },
                    {
                        ref: '#',
                        navTopic: 'news'
                    },
                    {
                        ref: '#',
                        navTopic: 'shop'
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .container{
        height: 90px;
    }
    .container>div{
        height: 80px;
        width: 80px;
    }
    ul a {
        text-decoration: none;
        text-transform: uppercase;
        color: black;
        height: 90px;
        display: inline-block;
        line-height: 90px;
        border-bottom: 2px solid transparent;
        
        &:hover{
        border-bottom: 2px solid #0d6efd;
        color: #0d6efd;
        }
    }
</style>