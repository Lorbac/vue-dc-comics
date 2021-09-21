<template>
  <main>
    <div class="jumbotrone">
      <img src="https://www.dccomics.com/sites/default/files/dc-hero_20210920_DCFD_ImpermananceBatman_6148def529b0e2.09931422.jpg" alt="">
    </div>
    <div class="container">
      <div class="series-banner">
        <h2>CURRENT SERIES</h2>
      </div>
      <ComicsBooks
        v-for="(comic, index) in comics"
        :key="index"
        :com="comic"
      />
      <button class="load-more-button">
        LOAD MORE
      </button>
    </div>
    <div class="container-band">
    <BlueBand 
      v-for="(img, i) in content"
      :key="i"
      :cont="img"  
    />
    </div>
  </main>
</template>

<script>
import ComicsBooks from "@/components/ComicsBooks.vue"
import ComicsItem from "@/data/ComicsItem.js"
import BlueBand from "@/components/BlueBand.vue"
import PaneContent from "@/data/PaneContent.js"

export default {
  name: 'Main',
  components: {
    ComicsBooks,
    BlueBand
  },
  data() {
    return{
      comics : ComicsItem,
      content: PaneContent
    } 
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  main {
    background-color: #1C1C1C;

    .jumbotrone {
      width: 100%;

      img{
        width: 100%;
        height: 400px;
        object-fit: cover;
        object-position: top;
      }
    }

    .container {
      position: relative;
      display: flex;
      flex-wrap: wrap;
      width: 70%;
      margin: 0 auto;
      padding: 50px 0;

      .series-banner {
        position: absolute;
        top: -22px;
        left: -10px;
        height: 45px;
        line-height: 45px;
        background-color: #0282F9;
        color: white;
        padding: 0 20px;

        h2 {
          font-size: 20px;
        }
      }

      .load-more-button {
        background-color: #0282F9;
        color: white;
        font-weight: 600;
        font-size: 15px;
        padding: 10px 50px;
        margin: 0 auto;
        margin-top: 20px;
        cursor: pointer;
      }
    }

    .container-band {
      display: flex;
    }
  }
</style>
