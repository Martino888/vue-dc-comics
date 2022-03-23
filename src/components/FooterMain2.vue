<template>
    <div class="socials">
        <div class="container">
            <div class="btn">
                <a href="">SIGN-UP NOW!</a>
            </div>
            <div class="left_icons">
                <h4>FOLLOW US</h4>
                <img src="../assets/img/footer-facebook.png" alt="logo grigio Facebook">
                <img src="../assets/img/footer-twitter.png" alt="logo grigio Twitter">
                <img src="../assets/img/footer-youtube.png" alt="logo grigio Youtube">
                <img src="../assets/img/footer-pinterest.png" alt="logo grigio Pinterest">
                <img src="../assets/img/footer-periscope.png" alt="logo grigio simbolo posizione">
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">

.socials {
    display: flex;
    background-color: #303030;
    padding: 1rem 35px;
    align-items: center;
    }

.container{
    display: flex;
}

h4{
    margin-right: 50px;
    margin-left: 32em;
    color:rgb(7, 149, 206) ;
}

a{
    color: white;
    text-decoration: none;
}

img{
    padding:15px
    }

.btn {
    border: 2px solid rgb(7, 149, 206) ;
        padding: 1rem 25px;
    }
.left_icons {
    display: flex;
    margin-right: 1rem;
}
</style>
