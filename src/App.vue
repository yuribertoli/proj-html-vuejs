<template>
  <div id="app">
    <MyHeader :navbar='headerNavbar'/>
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
      headerNavbar: [ //creo un array di oggetti per popolare dinamicamente la navbar dell'header
        {url: "#", name: "Contacts"},        
        {url: "#", name: "Info"},        
        {url: "#", name: "Shop"}        
      ]
    }
  }
}
</script>

<style lang="scss">
@import "./assets/style/general.scss";
</style>
