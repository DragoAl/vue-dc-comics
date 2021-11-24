<template>
<section>
    <ul>
        <li v-for="info, y in infos" :key='y'>
            <img :src="require(`../assets/img/${info.img}`)" :alt="info.text">  
            <a :href="info.url"> {{info.text}}</a>

        </li>
    </ul>

</section>
    
    
</template>

<script>
export default {
    name: 'PanelMenu',
    data(){
        return {
            infos: [
                {
                    text:'DIGITAL COMICS',
                    url: '#',
                    img : 'buy-comics-digital-comics.png'
                    
                },
                {
                    text:'DC MERCHANDISE',
                    url: '#',
                    img:"buy-comics-merchandise.png"
                },
                {
                    text:'SUBSCRIPTION',
                    url: '#',
                    img : "buy-comics-subscriptions.png"
                },
                {
                    text:'COMIC SHOP LOCATOR',
                    url: '#',
                    img : "buy-comics-shop-locator.png"
                },
                {
                    text:'DC POWER VISA',
                    url: '#',
                    img : "buy-dc-power-visa.svg"
                }
            ]


        }
    }
}
</script>

<style scoped lang="scss">
section {
    background-color: #0282f9;

    ul {
    display: flex;
    padding: 15px 10px;
    width: 75%;
    margin: 0px auto;
    display: flex;
    justify-content: space-around;


    li {
        // width: calc(100% / 5 ) ;
        list-style: none;
        padding: 20px;
        display: flex;
        align-items: center;
        // justify-content: space-around;
        // margin: 0 10px;

        
        img {
            // width: 40px;
            height: 40px;
            
        }

        a{
            text-decoration: none;
            color: white;
            font-size: 10px;
            margin-left: 8px;
        }

    }
}

}


</style>