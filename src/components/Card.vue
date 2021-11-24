<template>
  <div class="comic-card">
    <div class="image">
        <img :src="url" alt="title">
    </div>
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
        h3 {
            text-transform: uppercase;
            font-size: 12px;
        }
        .image {
            width: 100%;
            height: 170px;
            margin-bottom: 1rem;
            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top;
            }
        }
        
    }
</style>


