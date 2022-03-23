<template>
    <header>
        <div class="contain">
            <img class="logo" src="@/assets/img/dc-logo.png" alt="">
            <ul>
                <li v-for="(link, index) in links" :key="index" class="list_active"><a :href="link.href">{{link.text.toUpperCase()}}</a></li>
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
                text: 'characters'
            },
            {
                href: '#',
                text: 'comics'
            },
            {
                href: '#',
                text: 'movies'
            },
            {
                href: '#',
                text: 'tv'
            },
            {
                href: '#',
                text: 'games'
            },
            {
                href: '#',
                text: 'collectibles'
            },
            {
                href: '#',
                text: 'videos'
            },
            {
                href: '#',
                text: 'fans'
            },
            {
                href: '#',
                text: 'news'
            },
            {
                href: '#',
                text: 'shops'
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

    .contain{
        display:flex;
        align-items:center;
        justify-content: space-around;
        background-color: white;
        width: 100%;
    }

    li{
        display:inline-block;
        padding: 15px;
    }

    a{
        text-decoration:none;
        color:rgb(63, 61, 61);
        font-size: x-small;
    }

    a:hover{
        color:rgb(0, 119, 255);
    }

    .logo{
        width: 100px;
        padding:13px;
    }

    .here{
        width: 100%;
        background-color: black;
        color:white;
    }

    .list_active:hover {
        color: rgb(0, 119, 255);
        &::after {
        content: "";
        display: block;
        width: 50px;
        height: 5px;
        background-color: rgb(0, 119, 255);
        margin: auto;
        margin-top: 2rem;
            margin-bottom: -36px;
    }
    }
</style>
