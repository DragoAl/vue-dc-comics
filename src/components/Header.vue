<template>
    <header>
        <img src="../assets/img/dc-logo.png" alt="logo dc comics">
        <ul>
            <li v-for="link, i in links" :key='i'>
                <a :href="link.url" :class="link.isActive ? 'active' : '' ">{{link.text}}</a>

            </li>
        </ul>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'COMICS',
                    url: '#',
                    isActive: true
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'TV',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'GAMES',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'FANS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'NEWS',
                    url: '#',
                    isActive: false
                },
                {
                    text: 'SHOP',
                    url: '#',
                    isActive: false
                }
            ]
        }
    }
}
</script>

<style scoped lang="scss">
    header {
        width: 70%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        
        img {
            width: 7%;
        }
        
        li {
            display:inline-block;
            margin: 0 8px;
            a {
                text-decoration: none;
                color: #494b68;
                font-size: 10px;
                font-weight: bold;
                
                &.active {
                    color: #0282f9 ;
                }
            }
        }
    }


</style>