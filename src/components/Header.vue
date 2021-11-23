<template>
    <header>
        <div class="container">
            <div class="columns">
                <div class="brand">
                    <img src="@/assets/img/dc-logo.png" alt="logo">
                </div>

                <nav>
                    <ul>
                        <li v-for="(link, index) in navlist" :key="`link-${index}`"
                        :class="{active: link.current}"
                        @click="setCurrentLink(index)"
                        > 
                            <a :href="link.url"> {{ link.text }} </a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>    
    </header>
</template>

<script>
export default {
    name: 'Header',
    data () {
        return {
            
            navlist: [
                {
                    text: 'Characters',
                    url: '/Characters',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '/Comics',
                    current: false,
                },
                {
                    text: 'Movies',
                    url: '/Movies',
                    current: false,
                },
                {
                    text: 'Tv',
                    url: '/Tv',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '/Games',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '/Collectibles',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '/Videos',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '/Fans',
                    current: false,
                },
                {
                    text: 'News',
                    url: '/News',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '/Shop',
                    current: false,
                },
            ],
        }
    },

    methods: {
        setCurrentLink(index) {
            this.navlist.forEach((link) => {
                link.current = false;
            })
            this.navlist[index].current = true;
        }
    }
}
</script>

<style lang="scss" scoped>
    .columns {
        height: 100px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        nav {
            height: 100%;
        }
            ul {
                height: 100%;
                list-style: none;
                display: flex;
                align-items: center;
                li {
                    display: flex;
                    align-items: center;
                    height: 100%;
                    font-size: .8rem;
                    margin: 1em;
                    text-transform: uppercase;
                    border-bottom: 5px solid transparent;
                    cursor: pointer;
                    &:hover,
                    &.active {
                        border-bottom-color: #0c7cec;
                        & a {
                            color: #0c7cec;
                        }
                    }

                }
            }
    }


    .brand {
        display: flex;
        align-items: center;
        img {
            width: 80%;
        }
    }
</style>

