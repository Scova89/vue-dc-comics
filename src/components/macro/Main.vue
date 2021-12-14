<template>
<div class="container">
    <div class="main-sup">
        <Fumetti/>
    </div>
    <div class="main-inf">
        <ul>
            <li v-for="(link, index) in links" :key="index">
                <a :href="link.url"><img :src="link.icon" alt=""><span>{{link.text}}</span></a></li>
        </ul>
    </div>
</div>
  
</template>

<script>
import Fumetti from './sections/Fumetti.vue';
export default {
    name: 'Main',
    components: {
        Fumetti
    },
    data () {
        return {
            links: [
                {
                    icon: require("../../assets/img/buy-comics-digital-comics.png"),
                    text: "digital comics",
                    url: "#",
                    current: false,
                },
                {
                    icon: require("../../assets/img/buy-comics-merchandise.png"),
                    text: "dc merchandise",
                    url: "#",
                    current: false,
                },
                {
                    icon: require("../../assets/img/buy-comics-subscriptions.png"),
                    text: "subscription",
                    url: "#",
                    current: false,
                },
                {
                    icon: require("../../assets/img/buy-comics-shop-locator.png"),
                    text: "comic shop locator",
                    url: "#",
                    current: false,
                },
                {
                    icon: require("../../assets/img/buy-dc-power-visa.svg"),
                    text: "dc power visa",
                    url: "#",
                    current: false,
                },
                  
            ]
        }
    }

}
</script>

<style lang="scss">
    .main-sup{
        background-color: rgb(28 28 28);
        
        p{
            color: white;
            padding: 50px;
        }
    }

    .main-inf{
        background-color: rgb(2 130 249);
        height: 200px;
        display: flex;
        justify-content: space-evenly;
        align-items: center;

        ul{
            display: flex;
            list-style: none;
            
            

            li{
                
            
                a{
                text-decoration: none;
                color: white;
                padding: 0 30px;
                
                    span{
                        font-family: Arial, Helvetica, sans-serif;
                        text-transform: uppercase;
                        font-size: 9pt;
                    }

                    img{
                        height: 40px;
                        margin-right: 10px;
                        object-fit: cover;
                    }

                
                }
            }

            
        }
    }

</style>