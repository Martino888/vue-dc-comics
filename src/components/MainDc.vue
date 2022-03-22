<template>
    <main>
        <div class="container">
            <h3>{{text}}</h3>
        </div>
        <div class="logosm">
            <ul>
                <li v-for="(link, index) in links" :key="index"><a :href="link.href">{{link.text}}</a></li>
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

.container {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: black;
    color: white;
    height: 70px;
}
li{
    display:inline-block;
    padding: 5px;
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
    background-color:blue;
    color: white;
    height: 100px;
}
</style>
