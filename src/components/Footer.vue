<template>
  <footer>
    <div class="top-footer">
      <div class="left-side-top-footer">
        <div class="dc-comics-shop">
          <h2>DC COMICS</h2>
          <ul>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
          <h2>SHOP</h2>
          <ul>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="dc">
          <h2>DC</h2>
          <ul>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy policy (New)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptio</a></li>
            <li><a href="#">Talent Workshop</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>
        </div>
        <div class="sites">
          <h2>SITES</h2>
          <ul>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazines</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
      <div class="right-side-top-footer">

      </div>
    </div>
    <div class="bottom-footer">
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .top-footer {
    display: flex;
    justify-content: space-around;
    height: 400px;
    width: 100%;
    background-image: url(../assets/images/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    .left-side-top-footer {
      display: flex;
      justify-content: center;
      height: 100%;
      padding: 40px;
      padding-left: 200px;

      div {
        margin: 0 25px;

        h2 {
          color: white;
          font-size: 20px;
        }
      }

      ul {
        list-style: none;

        li {
          text-decoration: none;
          margin: 5px 0;

          a {
            color: rgb(89, 89, 89);
            text-decoration: none;
            font-size: 14px;
            
            &:hover {
              color: #0282F9;
            }
          }
        }
      }
    }

    .right-side-top-footer {
      height: 100%;
      min-width: 40%;
      background-image: url(../assets/images/dc-logo-bg.png);
      background-repeat: no-repeat;
      background-position: center;
      background-size: 550px;
    }
  }

  .bottom-footer {
    height: 150px;
    width: 100%;
    background-color: #303030;
  }
</style>
