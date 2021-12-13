<template>
  <header>
      <div class="logo">
          <img src="../assets/img/dc-logo.png" alt="">
      </div>
      
      <nav>
          <ul>
              <li v-for="(link, index) in links" :key="index"><a :href="link.url">{{link.text}}</a></li>
          </ul>
      </nav>
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

<style>
    header{
        display: flex;
        justify-content: space-between;
    }

</style>