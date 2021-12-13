<template>
<div class="container">
    <div class="main-sup">
        <p>--Contents goes here--</p>
    </div>
    <div class="main-inf">
        <ul>
            <li v-for="(link, index) in links" :key="index"><a :href="link.url"><img :src="link.icon" alt="">{{link.text}}</a></li>
        </ul>
    </div>
</div>
  
</template>

<script>
export default {
    name: 'Main',
    data () {
        return {
            links: [
                {
                    icon: "./img/buy-comics-digital-comics.png",
                    text: "digital comics",
                    url: "#",
                    current: false,
                },
                {
                    text: "dc merchandise",
                    url: "#",
                    current: false,
                },
                {
                    text: "subscription",
                    url: "#",
                    current: false,
                },
                {
                    text: "comic shop locator",
                    url: "#",
                    current: false,
                },
                {
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

        ul{
            display: flex;
            list-style: none;
            justify-content: space-evenly;
            padding: 50px;

            a{
                text-decoration: none;
                color: white;
                padding-bottom: 30px;

                img{
                    height: 50px;
                    object-fit: cover;
                }

                
            }
        }
    }

</style>