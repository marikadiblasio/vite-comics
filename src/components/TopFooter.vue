<template>
    <footer>
       <div class="container d-flex justify-content-between">
        <div class="text-white">
            <ul class="list-unstyled py-4">
                <li>cip</li>
            </ul>
            <ul>
                <li>cip</li>
            </ul>
            <ul>
                <li>cip</li>
            </ul>
            <ul>
                <li>cip</li>
            </ul>
        </div>
        <div class="w-25"><img class="w-100" src="../assets/img/dc-logo-bg.png" alt="logo"></div>
       </div> 
    </footer>
</template>

<script>
    export default {
        name: 'TopFooter'
    }
</script>

<style lang="scss" scoped>
    footer {
        background-image: url('../assets/img/footer-bg.jpg');
        height: 300px;
        overflow: hidden;
    }
    img {
        object-position: center -15px;
    }
</style>