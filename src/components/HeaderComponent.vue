<template>
    <header class="bg-white">
        <div class="container d-flex justify-content-between py-2 align-items-center">
            <div><img src="../assets/img/dc-logo.png" alt="Logo"></div>
            <nav>
                <ul class="d-flex list-unstyled">
                    <li class="pe-2"><a href="">nav ancora</a></li>
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