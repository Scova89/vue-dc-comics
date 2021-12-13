<template>
  <header>
      <div class="container">
        <div class="logo">
          <img src="../assets/img/dc-logo.png" alt="">
        </div>
      
        <nav>
          <ul>
            <li v-for="(link, index) in links" :key="index"><a :href="link.url">{{link.text}}</a></li>
          </ul>
        </nav>
      </div>
      
  </header>
</template>

<script>
export default {
    name: 'Header',
    data () {
        return {
            links: [
                {
                    text: "characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "comics",
                    url: "#",
                    current: false,
                },
                {
                    text: "movies",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss">
    header{
        .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px 0;

            img{
                width: 70%;
            }
        }
    }

    nav{
        ul{
            display: flex;
            list-style: none;
            

            a{
                text-decoration: none;
                margin: 0 10px;
            }
        }
    }

</style>