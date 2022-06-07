<template>
    <header class="header">
        <img src="../../assets/style/IMG/spotify-logo.png" alt="">
    </header>
</template>

<script>


export default {
    name: 'BaseHeader',
}
</script>


<style lang='scss' scoped>
    header {
        display: flex;
        height: 50px;
        background-color: #2e3a46;

        img {
            padding: 5px;
        }
    }
</style>