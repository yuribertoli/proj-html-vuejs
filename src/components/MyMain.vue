<template>
  <main>
      <MyJumbotron/>
      <ProBarbers/>
  </main>
</template>

<script>
import MyJumbotron from "./partialsMain/MyJumbotron.vue";
import ProBarbers from "./partialsMain/ProBarbers.vue"

export default {
    name: "MyMain",

    components: {
        MyJumbotron,
        ProBarbers
    },

    data(){
        return{

        }
    },

    methods: {
        
    }
}
</script>

<style lang="scss" scoped>

</style>