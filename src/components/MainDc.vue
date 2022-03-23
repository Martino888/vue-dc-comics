<template>
    <main>
        <div class="container">
            <h3>{{text}}</h3>
        </div>
        <div class="logosm">
            <ul>
                <li v-for="(link, index) in links" :key="index"><a :href="link.href">{{link.text}}<img src="" alt=""></a></li>
            </ul>
        </div>
    </main>
</template>

<script>
/* eslint-disable */
export default {
    name: "MainDc",
    data(){
        return {
            text:"--> Content goes here<--",
            links:[
            {
                img:"../assets/img/buy-comics-digital-comics.png",
                href: '#',
                text: 'CHARACTERS'
            },
            {
                img:"../assets/img/buy-comics-digital-comics.png",
                href: '#',
                text: 'COMICS'
            },
            {
                img: "../assets/img/buy-comics-digital-comics.png",
                href: '#',
                text: 'MOVIES'
            },
            {
                img: "../assets/img/buy-comics-digital-comics.png",
                href: '#',
                text: 'TV'
            },
            {
                img: "../assets/img/buy-comics-digital-comics.png",
                href: '#',
                text: 'GAMES'
            },
            ]
        }
    }
};
</script>

<style scoped lang="scss">
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

h3{
    margin-left: 10%;
}

.container {
    display: flex;
    align-items: center;
    background-color: black;
    color: white;
    height: 70px;
}
li{
    display:inline-block;
    padding: 15px;
}

a{
        text-decoration:none;
        color: white;
    }

    a:hover{
        color:blue;
    }


.logosm{
    display: flex;
    text-decoration: none;
    align-items: center;
    justify-content: center;
    background-color:rgb(7, 149, 206);
    color: white;
    height: 100px;
}
</style>
