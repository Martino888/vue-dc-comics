<template>
    <main>
        <div class="jambo"></div>
        <div class="btn">
            <button class="btin" href="">CURRENT SERIES</button>
        </div>
        <div class="card">
            <CardDc v-for="card in cards" :key="card.series"  :book-thumb="card.thumb" :book-titolo="card.series"  />
        </div>
        <div class="btn-more">
            <button class="btin2" href="">LOAD MORE</button>
        </div>
        <div class="logosm">
            <ul>
                <li v-for="(link, index) in links" :key="index"><a :href="link.href">{{link.text}}</a><img class="locandina" :src="link.img" alt=""></li>
            </ul>
        </div>
    </main>
</template>

<script>
import ImgDC from '../assets/img/buy-comics-digital-comics.png'
import ImgDC1 from '../assets/img/buy-comics-merchandise.png'
import ImgDC2 from '../assets/img/buy-comics-shop-locator.png'
import ImgDC3 from '../assets/img/buy-comics-subscriptions.png'
import ImgDC4 from '../assets/img/buy-dc-power-visa.svg'
import CardDc from './CardDc.vue'
/* eslint-disable */
export default {
    name: "MainDc",
    components: {
        CardDc
    },
    data(){
        return {
            cards:[
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                price: "$19.99",
                series: "Action Comics",
                type: "comic book"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                price: "$3.99",
                series: "American Vampire 1976",
                type: "comic book"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                price: "$16.99",
                series: "Aquaman",
                type: "graphic novel"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                price: "$2.99",
                series: "Batgirl",
                type: "comic book"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                price: "$3.99",
                series: "Batman",
                type: "comic book"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                price: "$2.99",
                series: "Batman Beyond",
                type: "comic book"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                price: "$3.99",
                series: "Batman/Superman",
                type: "comic book"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                price: "$4.99",
                series: "Batman/Superman Annual",
                type: "comic book"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                price: "$5.99",
                series: "Batman: The Joker War Zone",
                type: "comic book"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                price: "$6.99",
                series: "Batman: Three Jokers",
                type: "comic book"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                price: "$4.99",
                series: "Batman: White Knight Presents: Harley Quinn",
                type: "comic book"
            },
            {
                thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                price: "$16.99",
                series: "Catwoman",
                type: "graphic novel"
            }
        ],
            links:[
            {
                img: ImgDC,
                href: '#',
                text: 'CHARACTERS'
            },
            {
                img:ImgDC1,
                href: '#',
                text: 'COMICS'
            },
            {
                img: ImgDC2,
                href: '#',
                text: 'MOVIES'
            },
            {
                img: ImgDC3,
                href: '#',
                text: 'TV'
            },
            {
                img: ImgDC4,
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
main{
    background-color: black;
}

.card{
    margin: 46px;
    display: flex;
    flex-wrap:wrap;
    color: white;
}

.locandina {
    width: 40px;
    height: 40px;
    align-items: center;
}

.jambo {
    background-image:url("../assets/img/jumbotron.jpg");
    background-size: cover;
    color: white;
    height: 300px;
}
li{
    display:inline-block;
    padding: 55px;
}

a{
        text-decoration:none;
        color: white;
    }

    a:hover{
        color:rgb(7, 149, 206);
    }

.btn{
        background: rgb(7, 149, 206);
    display: inline-block;
    height: 33px;
    margin-left: 46px;
}

.btin{
        padding: 10px;
    color: white;
    background-color: rgb(7, 149, 206);
    border:none;
    font-size:30px;
}

.btin2{
        padding: 10px;
    color: white;
    background-color: rgb(7, 149, 206);
    border:none;
    margin-bottom: 20px;
        width: 200px;
}

.btn-more{
    display: flex;
    align-items: center;
    justify-content: center;

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
