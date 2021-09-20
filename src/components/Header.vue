<template>
  <div class="nav">
    <div class="nav-logo">
      <img src="../assets/images/dc-logo.png" alt="">
    </div>
    <div class="nav-menu">
      <ul>
        <li :class="(link.current) ? 'active' : 'null'"  v-for="(link, index) in links" :key='index'>
          <a :class="(link.current) ? 'active' : 'null'" :href="link.url">
          {{ link.text }}
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',

  data() {
    return {
      links : [
        {
          text: "CHARACTER",
          url: "#",
          current: false
        },
        {
          text: "COMICS",
          url: "#",
          current: true
        },
        {
          text: "MOVIES",
          url: "#",
          current: false
        },
        {
          text: "TV",
          url: "#",
          current: false
        },
        {
          text: "GAMES",
          url: "#",
          current: false
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          current: false
        },
        {
          text: "VIDEOS",
          url: "#",
          current: false
        },
        {
          text: "FANS",
          url: "#",
          current: false
        },
        {
          text: "NEWS",
          url: "#",
          current: false
        },
        {
          text: "SHOP",
          url: "#",
          current: false
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .nav {
    display: flex;
    justify-content: space-around;
    width: 100%;
    height: 100px;
    padding: 10px;

    .nav-logo img {
      height: 100%;
    }

    .nav-menu ul {
      list-style: none;
      display: flex;
      justify-content: center;

      li {
        &:hover,
        &.active {
          transition: linear 0.2s;
          border-bottom: 5px solid #0282F9;
          padding-bottom: 5px;
        }

        a {
          display: inline-block;
          margin: 30px 20px 30px 20px;
          text-decoration: none;
          font-size: 0.99rem;
          font-weight: 600;
          color: rgb(68, 68, 68);

          &:hover,
          &.active {
            color: #0282F9;
          }
            
        }
      }
    }
  }
</style>
