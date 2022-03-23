<template>
    <div class="container">
        <img :src="bookThumb" :alt="bookTitolo">
        <h3>{{ bookTitolo }}</h3>
    </div>
</template>

<script>
export default {
  name: 'CardDc',
  props: {
    bookThumb: String,
    bookTitolo: String
  }
}
</script>

<style scoped lang="scss">
    .container{
        width: calc(100% /6);
        margin-top: 100px;
    }

    img {
        width: 178px;
        height: 178px;

    }
</style>
