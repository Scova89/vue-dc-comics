<template>
    <div class="container">
        <div class="footer-sup">
            <div class="list-container">
                <ul class="dc-comics-list">
                    <h2>dc comics</h2>
                    <li v-for="(dcComic, index) in dcComics" :key="index">
                        <a :href="dcComic.url">{{dcComic.text}}</a>
                    </li>
                </ul>

                <ul class="shops-list">
                    <h2>shop</h2>
                    <li v-for="(shop, index) in shops" :key="index">
                        <a :href="shop.url">{{shop.text}}</a>
                    </li>
                </ul>

                <ul class="dc-list">
                    <h2>dc</h2>
                    <li v-for="(dcBrand, index) in dcBrands" :key="index">
                        <a :href="dcBrand.url">{{dcBrand.text}}</a>
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
            ]
        }
    }
}
</script>

<style lang="scss">
    .footer-sup{
        background-image: url(../../assets/img/footer-bg.jpg);
        height: 500px;
        background-size: cover;
        display: flex;
        justify-content: space-between;

        h2{
            color: white;
        }

        a{
            font-family: Arial, Helvetica, sans-serif;
            color: white;
        }
    }

    .footer-inf{
        height: 100px;
        background-color: hsl(0deg 0% 19%);
    }

</style>