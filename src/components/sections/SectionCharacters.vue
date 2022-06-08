<template>
    <section>
        <div class="container">
            <div class="row">
                <CardCharacter class="col-12 col-sm-6 col-lg-3" v-for="(character, index) in characters" :key="index" :character="character"/>

            </div>
        </div>
    </section>
</template>

<script>
import axios from 'axios';
import CardCharacter from '../commons/CardCharacter.vue';

export default {
    name: 'SectionCharacters',
    data () {
        return {
            characters:[],
        };
    },
    components: {
        CardCharacter,
    },

    created() {
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')

        .then((response) => {
            // handle success
            this.characters = response.data.response;
            
        })

        .catch((error) => {
            // handle error
            console.log(error);
        })
    }
}
</script>

<style lang='scss' scoped>

</style>