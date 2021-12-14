<template>
    <section>
        <div class="comics-list">
            <div class="comics" v-for="comics in 12" :key="comics">
                ciao
            </div>
        </div>
    </section>
  
</template>

<script>
export default {
    name: 'Fumetti'
}
</script>

<style lang="scss" scoped>
    .comics-list{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;


        .comics{
        background-color: white;
        height: 200px;
        width: 25%;
        margin: 10px;
        }
    }

</style>