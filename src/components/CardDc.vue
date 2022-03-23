<template>
    <div>
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
    width: calc(100% /6);
</style>
