<template>
  <div id="app">
    <MyHeader :navbar='headerNavbar'/>
    <MyMain/>
    <MyFooter :cards='cardsFooter' :info='infoAvada' :socials='iconsSocials'/> 
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
        {url: "#", name: "Shop"},        
        {url: "#", name: "Info"},        
        {url: "#", name: "Contacts"}        
      ],

      cardsFooter: { //creo un oggetto che contiene le informazioni da passare ad ogni singola card tramite props
        shop: { 
                img: "avadabarbers_footer_shop_image-800x624.png", 
                alt: "barber products",
                text: "shop our range now", 
                url: "#"
              },
        book: { 
                img: "avadabarbers_footer_appointment_image-800x624.png",
                alt: "barber at work", 
                text: "book your appointment", 
                url: "#"
              }
      },

      infoAvada: [ //creo un array di oggetti da ciclare nel footer
        {name: "company-name", text: "Avada Barbers"},
        {name: "address", text: "123 New York Street"},
        {name: "town", text: "New York City"},
        {name: "email", text: "info@yourwebsite.com"},
        {name: "phone-number", text: "+1 (555) 555-1212"}
      ],

      iconsSocials: [ //utilizzo font awesome versione 5.15.4 per popolare le icone dei social media tramite classi dinamiche (dopo aver installato npm di font-awesome https://medium.com/front-end-weekly/how-to-use-fon-awesome-5-on-vuejs-project-ff0f28310821)
        {name: "Facebook", url: "#", class: "fab fa-facebook-f"},
        {name: "Twitter", url: "#", class: "fab fa-twitter"},
        {name: "YouTube", url: "#", class: "fab fa-youtube"},
        {name: "Instagram", url: "#", class: "fab fa-instagram"}
      ]
    }
  }
}
</script>

<style lang="scss">
@import "./assets/style/general.scss";
</style>
