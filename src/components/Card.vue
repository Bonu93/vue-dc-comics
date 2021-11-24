<template>
  <div class="comic-card">
    <img :src="url" alt="title">
    <h3>{{ title }}</h3>
  </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        url: String, 
        title: String,
    },

}
</script>

<style lang="scss" scoped>

    .comic-card {
        display: flex;
        flex-direction: column;
        img {
            width: 100%;
            height: 160px;
            object-fit: cover;
            object-position: top;

        }
        
    }
</style>


