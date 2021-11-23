<template>
    <footer>
        <div class="footer-nav">
            <div class="footer-lists">
                
            </div>

            <div class="dc-image">
                <img src="@/assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>

        <div class="footer-cta">

        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer', 
}
</script>

<style lang="scss" scoped>
    .footer-nav {
        height: 400px;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        display: flex;
    }

    .footer-cta {
        background-color: #303030;
        height: 100px;
    }

    .footer-lists {
        width: 50%;
    }

    .dc-image {
        overflow: hidden;
        width: 50%;
        // display: flex;
    }
    

    
</style>

