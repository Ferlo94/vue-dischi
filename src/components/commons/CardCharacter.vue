<template>
    <div class="character">
        <img src="https://images.agi.it/pictures/agi/agi/2021/04/22/213505783-2288da7e-bc71-4ffb-8227-9dcef7ca968a.png" alt="">
        <h6 class="titolo">TITOLO SONG</h6>
        <p class="autore">autore</p>
        <p class="data">data</p>
    </div>
</template>

<script>
export default {
    name: 'CardCharacter',
    props: {
        character: Object,
    }
}
</script>

<style lang='scss' scoped>
.character {
    text-align: center;
    background-color: #2e3a46;
    margin: 5px;

    img {
        max-width: 100%;
        padding: 10px;
    }

    h6 {
        color: white;
    }
    p {
        color: grey;
    }

}
</style>