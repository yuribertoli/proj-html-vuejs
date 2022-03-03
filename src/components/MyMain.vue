<template>
  <main>
      <MyJumbotron/>
      <ProBarbers/>
      <ServicesPart/>
      <GroomingProducts/>
  </main>
</template>

<script>
import MyJumbotron from "./partialsMain/MyJumbotron.vue";
import ProBarbers from "./partialsMain/ProBarbers.vue";
import ServicesPart from "./partialsMain/ServicesPart.vue";
import GroomingProducts from "./partialsMain/GroomingProducts.vue"

export default {
    name: "MyMain",

    components: {
        MyJumbotron,
        ProBarbers,
        ServicesPart,
        GroomingProducts
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