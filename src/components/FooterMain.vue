<template>
    <footer>
        <div class="container">
            <ul>
                <li><a href="#"><b class="title">DC COMICS</b> </a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">News</a></li>
            </ul>
            <ul>
                <li><a href="#"><b class="title">SHOP</b> </a></li>
                <li><a href="#">Shop DC</a></li>
                <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
        </div>
        <div>
            <ul>
                <li><a href="#"><b class="title">DC</b> </a></li>
                <li><a href="#">Terms Of Use</a></li>
                <li><a href="#">Privacy Policy (New)</a></li>
                <li><a href="#">Ad Choices</a></li>
                <li><a href="#">Advertising</a></li>
                <li><a href="#">Jobs</a></li>
                <li><a href="#">Subscriptions</a></li>
                <li><a href="#">Talent Workshops</a></li>
                <li><a href="#">CPSC Certificates</a></li>
                <li><a href="#">Ratings</a></li>
                <li><a href="#">Shop Help</a></li>
                <li><a href="#">Contact Us</a></li>
            </ul>
        </div>
        <div>
            <ul>
                <li><a href="#"><b class="title">SITES</b> </a></li>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD Magazine</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Power Visa</a></li>
            </ul>
        </div>
        <img src="../assets/img/dc-logo-bg.png" alt="">
    </footer>
</template>

<script>
/* eslint-disable */
export default {

}
</script>

<style scoped lang="scss">

.title {
    color: white;
    font-size:20px;
}

h3{
    color: white
}

li{
    text-decoration:none ;
    list-style-type: none;
}
a{
    text-decoration: none;
    color: grey;
}

footer{
    display:flex;
    background-image: url("../assets/img/footer-bg.jpg");
    background-position-x: center;
    justify-content: space-evenly;
}
</style>
