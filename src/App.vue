<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyMain from './components/MyMain.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',

  components: {
    MyHeader,
    MyMain,
    MyFooter
  },

  data(){
    return{
      header: [
        {url: "#", name: ""}
      ]
    }
  }
}
</script>

<style lang="scss">
@import "./assets/style/general.scss";
</style>
