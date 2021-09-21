<template>
    <div class="pane-content">
        <img :src="cont.image" :alt="cont.titolo">
        <h2>{{ cont.titolo.toUpperCase() }}</h2>
    </div>
</template>

<script>
export default {
    name:"BlueBand",
    props: ["cont"]
}
</script>

<style scoped lang="scss">
    .pane-content {
        width: 100%;
        height: 200px;
        background-color: #0282F9;
    }
</style>