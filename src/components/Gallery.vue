<template>
    
  <ul class="gallery">
      <li v-for="(comic, index) in comics" :key="`comic-${index}`">
         <Card :url="comic.thumb" :title="comic.series" />
      </li>
  </ul>
</template>

<script>
import dcComics from '@/data/dcComics.js'
import Card from '@/components/Card.vue'

export default {
    name: 'Gallery',
    components: {
        Card,
    },

    data () {
        return {
            comics: dcComics,
        }
    },
}
</script>

<style lang="scss" scoped>
    .gallery {
        display: flex;
        list-style: none;
        flex-wrap: wrap;
    } li {
        width: calc(100% / 6);
        display: flex;
        flex-direction: column;
        padding: .5rem;
    }
</style>
