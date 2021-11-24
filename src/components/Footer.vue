<template>
    <footer>
        <div class="container">
            <div class="footer-nav">
                <div class="col">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li v-for="(link, index) in dcComicsLinks" :key="`link-${index}`">
                            <a href="link.url">{{ link.text}}</a> 
                        </li>
                        
                    </ul>

                    <h4>SHOP</h4>

                    <ul>
                        <li v-for="(link, index) in shopLinks" :key="`link-${index}`"> 
                            <a href="link.url">{{ link.text}}</a> 
                        </li>
                        
                    </ul>
                </div>
                
                <div class="col">

                    <h4>DC</h4>

                    <ul>
                        <li v-for="(link, index) in dcLinks" :key="`link-${index}`"> 
                            <a href="link.url">{{ link.text}}</a> 
                        </li>
                    </ul>
                </div>

                <div class="col">

                    <h4>SITES</h4>

                    <ul>
                         <li v-for="(link, index) in sitesLinks" :key="`link-${index}`"> 
                            <a href="link.url">{{ link.text}}</a> 
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="footer-cta">
            <div class="container">
                
                    <div class="cta">
                        <button>Sign-up now!</button>
                    </div>

                    <div class="social">
                        <h4 class="">Follow us</h4>
                        <div class="social-links">
                            <img src="../assets/img/footer-facebook.png" alt="">
                            <img src="../assets/img/footer-periscope.png" alt="">
                            <img src="../assets/img/footer-pinterest.png" alt="">
                            <img src="../assets/img/footer-twitter.png" alt="">
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </div>
                    </div>
                
            </div>
        </div>
        
    </footer>
</template>

<script>
export default {
    name: 'Footer', 
    data () {
        return {
            dcComicsLinks: [
                {
                    text: 'Characters',
                    url: '/',
                },
                {
                    text: 'Comics',
                    url: '/',

                },
                {
                    text: 'Movies',
                    url: '/',

                },
                {
                    text: 'TV',
                    url: '/',

                },
                {
                    text: 'Games',
                    url: '/',

                },
                {
                    text: 'Videos',
                    url: '/',

                },
                {
                    text: 'News',
                    url: '/',

                },
            ],
            shopLinks: [
                {
                    text: 'Shop DC',
                    url: '/',
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '/',
                },
            ],
            dcLinks: [
                {
                    text: 'Terms of Use',
                    link: '/',
                },
                {
                    text: 'Privacy Policy (new)',
                    link: '/',
                },
                {
                    text: 'Ad Choices',
                    link: '/',
                },
                {
                    text: 'Advertising',
                    link: '/',
                },
                {
                    text: 'Jobs',
                    link: '/',
                },
                {
                    text: 'Subscription',
                    link: '/',
                },
                {
                    text: 'Talent Workshop',
                    link: '/',
                },
                {
                    text: 'CPSC Certificates',
                    link: '/',
                },
                {
                    text: 'Ratings',
                    link: '/',
                },
                {
                    text: 'Shop Help',
                    link: '/',
                },
                {
                    text: 'Contact Us',
                    link: '/',
                },
            ],
            sitesLinks: [
                {
                    text:'DC',
                    url: '/',
                },
                {
                    text:'Mad Magazine',
                    url: '/',
                },
                {
                    text:'DC Kids',
                    url: '/',
                },
                {
                    text:'DC Universe',
                    url: '/',
                },
                {
                    text:'DC Power Visa',
                    url: '/',
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
   @import '@/styles/footer.scss';
    
    
</style>

