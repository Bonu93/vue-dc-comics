<template>
  <div class="hero">
      <div class="container">
        <div class="label-container">
            <span class="label">CURRENT SERIES</span>
        </div>
      </div>
  </div>
      
</template>

<script>
export default {
    name: 'Hero',
}
</script>

<style lang="scss" scoped>
    .hero {
        height: 400px;
        background-image: url('../assets/img/jumbotron.jpg');
        .container {
            height: 100%;
        }
         .label-container {
            position: relative;
            top: 100%;
            left: -50px;
        } .label {
            display: inline-block;
            padding: 1rem 2rem;
            color: white;
            font-weight: 700;
            font-size: 1.5rem;
            background: #0282F9;
            transform: translateY(-50%);
        }
    } 
</style>