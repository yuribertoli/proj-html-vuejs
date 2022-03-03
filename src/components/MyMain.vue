<template>
  <main>
      <MyJumbotron/>
      <ProBarbers/>
      <ServicesPart/>
  </main>
</template>

<script>
import MyJumbotron from "./partialsMain/MyJumbotron.vue";
import ProBarbers from "./partialsMain/ProBarbers.vue";
import ServicesPart from "./partialsMain/ServicesPart.vue"

export default {
    name: "MyMain",

    components: {
        MyJumbotron,
        ProBarbers,
        ServicesPart
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