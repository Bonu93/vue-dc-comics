<template>
  <main>
      <div class="container">
           <Gallery />
      </div>
  </main>
</template>

<script>
import Gallery from '@/components/Gallery.vue'

export default {
    name: 'Main',
    components: {
        Gallery,
    },

    data () {
        return {
           
        }
    }
}
</script>

<style lang="scss" scoped>
   @import '@/styles/main'
</style>