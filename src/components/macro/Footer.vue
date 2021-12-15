<template>
    <div class="container">
        <div class="footer-sup">
            <div class="list-container container">
                <ul class="dc-comics-list">
                    <h2>dc comics</h2>
                    <li v-for="(dcComic, index) in dcComics" :key="index">
                        <a :href="dcComic.url">{{dcComic.text}}</a>
                    </li>
                    <ul class="shops-list">
                    <h2>shop</h2>
                    <li v-for="(shop, index) in shops" :key="index">
                        <a :href="shop.url">{{shop.text}}</a>
                    </li>
                </ul>
                </ul>

                <ul class="dc-list">
                    <h2>dc</h2>
                    <li v-for="(dcBrand, index) in dcBrands" :key="index">
                        <a :href="dcBrand.url">{{dcBrand.text}}</a>
                    </li>
                </ul>

                <ul class="sites">
                    <h2>sites</h2>
                    <li v-for="(site, index) in sites" :key="index">
                        <a :href="site.url">{{site.text}}</a>
                    </li>
                </ul>
            </div>

            <div class="logo-container">
            
            </div>
            
        </div>

        <div class="footer-inf">
            <button>sign-up now!</button>
            <div class="social-container">
                <h2>follow us</h2>
                <ul>
                    <li v-for="(social, index) in socials" :key="index">
                        <a :href="social.url"><img :src="social.icon" alt=""></a>
                    </li>
                </ul>
                
            </div>
        </div>
    </div>
  
  
</template>

<script>
export default {
    name: 'Footer',
    data () {
        return {
            dcComics: [
                {
                    text: "Characters",
                    url: "#",
                },
                {
                    text: "Comics",
                    url: "#",
                },
                {
                    text: "Movies",
                    url: "#",
                },
                {
                    text: "TV",
                    url: "#",
                },
                {
                    text: "Games",
                    url: "#",
                },
                {
                    text: "Videos",
                    url: "#",
                },
                {
                    text: "News",
                    url: "#",
                },
            ],

            shops: [
                {
                    text: "Shop DC",
                    url: "#",
                },
                {
                    text: "Shop DC Collectibles",
                    url: "#",
                },
            ],

            dcBrands: [
                {
                    text: "Terms of Use",
                    url: "#",
                },
                {
                    text: "Privacy Policies (New)",
                    url: "#",
                },
                {
                    text: "Ad Choices",
                    url: "#",
                },
                {
                    text: "Advertising",
                    url: "#",
                },
                {
                    text: "Jobs",
                    url: "#",
                },
                {
                    text: "Subscriptions",
                    url: "#",
                },
                {
                    text: "Talent Workshops",
                    url: "#",
                },
                {
                    text: "CPSC Certificates",
                    url: "#",
                },
                {
                    text: "Ratings",
                    url: "#",
                },
                {
                    text: "Shop Help",
                    url: "#",
                },
                {
                    text: "Contact Us",
                    url: "#",
                },
            ],

            sites: [
                {
                    text: "DC",
                    url: "#",
                },
                {
                    text: "MAD Magazine",
                    url: "#",
                },
                {
                    text: "DC Kids",
                    url: "#",
                },
                {
                    text: "DC Universe",
                    url: "#",
                },
                {
                    text: "DC Power Visa",
                    url: "#",
                },
            ],

            socials: [
                {
                    icon: require("../../assets/img/footer-facebook.png"),
                    url: "#",
                },
                {
                    icon: require("../../assets/img/footer-twitter.png"),
                    url: "#",
                },
                {
                    icon: require("../../assets/img/footer-youtube.png"),
                    url: "#",
                },
                {
                    icon: require("../../assets/img/footer-pinterest.png"),
                    url: "#",
                },
                {
                    icon: require("../../assets/img/footer-periscope.png"),
                    url: "#",
                },
            ]

        }
    }
}
</script>

<style lang="scss">
    .footer-sup{
        background-image: url(../../assets/img/footer-bg.jpg);
        height: 400px;
        background-size: cover;
        display: flex;
        justify-content: space-between;
        align-items: center;
        

        .list-container{
            
            height: 80%;
            display: flex;
            flex-wrap: wrap;

            ul{
                margin-right: 20px;
                

                h2{
                    color: white;
                    margin-top: 20px;
                }

                a{
                    font-family: Arial, Helvetica, sans-serif;
                    color: white;
                    font-size: 10pt;
                }


            }

        }

        .logo-container{
            width: 50%;
            height: 100%;
            background-image: url(../../assets/img/dc-logo-bg.png);
            background-size: cover;
            background-position-y: center;
            
        }
        
    }

    .footer-inf{
        padding: 0 30px;
        height: 100px;
        background-color: hsl(0deg 0% 19%);
        display: flex;
        justify-content: space-between;
        align-items: center;

        button{
            padding: 10px 20px;
            background-color: hsl(0deg 0% 19%);
            border: 2px solid rgb(2 130 249);
            cursor: pointer;
            color: white;
            text-transform: uppercase;
        }


        .social-container{
            display: flex;
            align-items: center;

            h2{
                color: rgb(2 130 249);
            }

            ul{
                display: flex;
                padding: 0 10px;

                li{
                    margin-left: 10px;
                }
            }
        }
    }

</style>