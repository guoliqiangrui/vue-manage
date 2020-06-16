<template>
  <div class="home">
    <ul>
      <li v-for="item in movieList" :key="item.id">
        <img :src="item.images.small">
        <span>{{item.title}}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      movieList: [
        {
          id: "1292052",
          title: "肖申克的救赎",
          images: {
            large: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p480747492.jpg",
            medium: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p480747492.jpg",
            small: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p480747492.jpg"
          }
        },
        {
          id: "1291546",
          title: "霸王别姬",
          images: {
            large: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2561716440.jpg",
            medium: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2561716440.jpg",
            small: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2561716440.jpg"
          }
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">

</style>
