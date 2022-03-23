<template>
    <header>
        <div class="header">.</div>
        <div class="container">
            <img class="logo" src="@/assets/img/dc-logo.png" alt="">
            <ul>
                <li v-for="(link, index) in links" :key="index"><a :href="link.href">{{link.text}}</a></li>
            </ul>
        </div>
    </header>

</template>

<script>
/* eslint-disable */
export default {
    name:'HeaderDc',
    data () {
        return {
            links:[
                {
                href: '#',
                text: 'CHARACTERS'
            },
            {
                href: '#',
                text: 'COMICS'
            },
            {
                href: '#',
                text: 'MOVIES'
            },
            {
                href: '#',
                text: 'TV'
            },
            {
                href: '#',
                text: 'GAMES'
            },
            {
                href: '#',
                text: 'COLLECTIBLES'
            },
            {
                href: '#',
                text: 'VIDEOS'
            },
            {
                href: '#',
                text: 'FANS'
            },
            {
                href: '#',
                text: 'NEWS'
            },
            {
                href: '#',
                text: 'SHOPS'
            }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
    *{
        margin:0;
        padding:0;
        box-sizing: border-box;
    }

    .header {
        background-color: black;
        height: 70px;
    }

    .container{
        display:flex;
        align-items:center;
        justify-content: space-around;
        background-color: white;
    }

    li{
        display:inline-block;
        padding: 5px;
    }

    a{
        text-decoration:none;
        color:black;
    }

    a:hover{
        color:blue;
    }

    .logo{
        width: 100px;
        padding:5px;
    }

    .here{
        width: 100%;
        background-color: black;
        color:white;
    }
</style>
