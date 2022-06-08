<template>
    <div class="character-card">
        <img :src="character.poster" :alt="character.title">
        <h6 class="titolo">{{character.title}}</h6>
        <p class="autore">{{character.author}}</p>
        <p class="year">{{character.year}}</p>
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
.character-card {
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