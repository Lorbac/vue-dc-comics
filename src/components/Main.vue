<template>
  <main>
    <h1>--> Content goes here &lt;-- </h1>
  </main>
</template>

<script>
export default {
  name: 'Main',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  main {
    height: 200px;
    background-color: black;
    display: flex;
    justify-content: center;
    align-items: center;

    h1 {
      color: white;
    }
  }
</style>
