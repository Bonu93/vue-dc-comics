<template>
  <div class="blue">
      <div class="container">
        <div class="feature">
            <div class="img-box">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            </div>
            <div class="img-txt">Digital comics</div>
        </div>
        <div class="feature">
            <div class="img-box">
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
            </div>
            <div class="img-txt">Dc merchandise</div>
        </div>
        <div class="feature">
            <div class="img-box">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            </div>
            <div class="img-txt">subscriptions</div>
        </div>
        <div class="feature">
            <div class="img-box">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            </div>
            <div class="img-txt">comic shop locator</div>
        </div>
        <div class="feature">
            <div class="img-box">
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            </div>
            <div class="img-txt">Dc power visa</div>
        </div>
        
      </div>
  </div>
</template>

<script>
export default {
    name: 'Bluebanner',
}
</script>

<style lang="scss" scoped>
    .blue {
        padding: 3rem 0;
        background-color: #0282F9;
        .container {
            display: flex;
            align-items: center;
            .feature {
                display: flex;
                align-items: center;
                color: white;
                width: calc(100% / 5);
                text-transform: uppercase;
                cursor: pointer;
                font-size: 14px;
            } .img-box {
                width: 30%;
                margin-right: 1rem;
                img {
                    height: 70px;
                }
            }
        }
    }
</style>