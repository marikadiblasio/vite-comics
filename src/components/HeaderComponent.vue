<template>
    <header class="bg-white">
        <div class="container d-flex justify-content-between py-2 align-items-center">
            <div><img src="../assets/img/dc-logo.png" alt="Logo"></div>
            <nav>
                <ul class="d-flex list-unstyled">
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
    ul a {
        text-decoration: none;
        text-transform: uppercase;
        color: black;
        padding-top: 3rem;
        padding-bottom: 3rem;
        border-bottom: 1px solid transparent;
    }
</style>