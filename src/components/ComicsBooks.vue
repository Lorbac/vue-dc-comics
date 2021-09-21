<template>
  <div class="comic-card">
      <img :src="com.thumb" :alt="com.type">
      <h3>{{ com.series.toUpperCase() }}</h3>
  </div>
</template>

<script>
export default {
    name: 'ComicsBooks',
    props: ['com']
}
</script>

<style scoped lang="scss">
    .comic-card {
        flex-basis: calc((100% / 6));
        background-color: #1C1C1C;
        padding: 10px 10px;
        
        img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            object-position: top;
            cursor: pointer;
        }

        h3 {
            color: white;
            font-size: 15px;
        }
    }
</style>