<template>
    <footer>
        <div class="container">
            <div class="footer-nav">
                <div class="col">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                    </ul>

                    <h4>SHOP</h4>

                    <ul>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                    </ul>
                </div>
                
                <div class="col">

                    <h4>DC</h4>

                    <ul>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                    </ul>
                </div>

                <div class="col">

                    <h4>SITES</h4>

                    <ul>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                        <li>
                            <a href="">Characters</a> 
                        </li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="container">
            <div class="footer-cta">

            </div>
        </div>

        
    </footer>
</template>

<script>
export default {
    name: 'Footer', 
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
            background-size:auto;
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

    h4 {
        margin: 1rem 0;
    }

    
    
</style>

