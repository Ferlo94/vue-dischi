<template>
    <main>
        <SectionCharacters/>
    </main>
</template>

<script>
import SectionCharacters from '../sections/SectionCharacters.vue';
export default {
  name: 'BaseMain',  
  components: { SectionCharacters 
  },
    
}
</script>

<style lang='scss'>
main{
    background-color: #1e2d3b;
}
</style>