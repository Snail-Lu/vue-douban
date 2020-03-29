<template>
    <div class="navbar">
        <ul class="flex">
            <li class="navbar-item flex-item-1" v-for="(item,index) in navbarList" :key="index">{{item}}</li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'Navbar',
        data: function(){
            return {
                navbarList: ['首页','书影音','小组','市集','我的'],
            }
        },
        props: {

        }
    }
</script>

<style lang="scss" scoped>
    .navbar{
        position: fixed;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 2rem;
        line-height: 2rem;
        border-top: 1px solid #eee;
        .navbar-item{
            font-size: 1rem;
            transform: scale(0.5);
            -webkit-transform: scale(0.5);
            // zoom: 0.5;
            transform-origin: center;
        }
    }
</style>
