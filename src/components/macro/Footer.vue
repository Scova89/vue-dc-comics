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
                    <h2>dc</h2>
                    <li v-for="(site, index) in sites" :key="index">
                        <a :href="site.url">{{site.text}}</a>
                    </li>
                </ul>
            </div>

            <div class="logo-container">
                <img src="../../assets/img/dc-logo-bg.png" alt="dc-logo-bg">
            </div>
            
        </div>

        <div class="footer-inf">
            
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

        
    }

    .footer-inf{
        height: 100px;
        background-color: hsl(0deg 0% 19%);
    }

</style>