<template>
    <header>
        <div class="container">
            <div class="columns">
                <!-- <div class="brand"> -->
                    <img src="@/assets/img/dc-logo.png" alt="logo">
                <!-- </div> -->

                <!-- <nav> -->
                    <ul>
                        <li v-for="(link, index) in navlist" :key="`link-${index}`"
                        :class="{active: link.current}"
                        @click="setCurrentLink(index)"
                        > 
                            <a :href="link.url"> {{ link.text }} </a>
                        </li>
                    </ul>
                <!-- </nav> -->
            </div>
        </div>    
    </header>
</template>

<script>
import navList from '@/data/navList.js'

export default {
    name: 'Header',
    
    data () {
        return {
            
            navlist: navList,
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
    @import '@/styles/header'
    
</style>

