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
    footer {
        color: white;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        .footer-nav {
            display: flex;
            padding: 2rem 0;
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-position-x: right;
            background-position-y: center;
            background-size: 45%;
            .col {
                margin-right: 2rem;
                ul {
                    list-style: none;
                    font-size: .7rem;
                    li {
                        display: flex;
                        margin: 5px 0;
                        a {
                            color: grey;
                        }
                    }
                }
            }
        }
    
    }

    .footer-cta {
        background-color: #303030;
        padding: 2rem;
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            .cta {
                button {
                        cursor: pointer;
                        background: transparent;
                        color: white;
                        border: 3px solid #0282F9;
                        text-transform: uppercase;
                        padding: 1rem;
                    }
            }
            .social {
                display: flex;
                align-items: center;
                h4 {
                    color: #0282F9;
                    text-transform: uppercase;
                }
                .social-links {

                    img {
                        margin: 0 .5rem;
                    }
                }
            }
        }
    }

    h4 {
        margin: 1rem 0;
    }

    
    
</style>

