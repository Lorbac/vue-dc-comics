<template>
  <footer>
    <div class="top-footer">
      <div class="left-side-top-footer">

      </div>
      <div class="right-side-top-footer">
        <img src="../assets/images/dc-logo-bg.png" alt="">
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
      width: 50%;
      height: 100%;
    }

    .right-side-top-footer {
      width: 50%;
      height: 100%;
      position: relative;
      
      img {
      position: absolute;
      opacity: 0.9;
      width: 60%;
      height: 100%;
      object-fit: cover;
      }
    }
  }

  .bottom-footer {
    height: 150px;
    width: 100%;
    background-color: #303030;
  }
</style>
