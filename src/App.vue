<template>
  <div id="app">
    <app-header />
    <main>
      <app-products />
    </main>
    <app-footer :pasta = "pastificio" />
  </div>
 
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppProducts from './components/AppProducts.vue'
import AppFooter from './components/AppFooter.vue'
export default {
  name: 'App',
  components: {
    AppHeader,
    AppProducts,
    AppFooter
  },
  data(){ 
    return {
      links: [
                {
                    text: "Home",
                    url: "#",
                    active: false,
                },
                {
                    text: "Prodotti",
                    url: "#",
                    active: true,
                },
                {
                    text: "Chi Siamo",
                    url: "#",
                    active: false,
                },
                {
                    text: "Contatti",
                    url: "#",
                    active: false,
                },
            ],

      pastificio:[
               {
                    text: "il pastificio",
                    url: "#",
                    active: false,
                },
                {
                    text: "Grano",
                    url: "#",
                    active: false,
                },
                {
                    text: "filiera",
                    url: "#",
                    active: false,
                },
                {
                    text: "100 anni di pasta",
                    url: "#",
                    active: false,
                },
                {
                    text: "Sartoria della pasta",
                    url: "#",
                    active: false,
                },
        
      ]
     
    
    }
  },
  methods:{
  }
}
</script>

<style lang="scss">
@import "./style/vars";
@import "./style/generals";
@import "./style/utilities";
h1,
h2,
h3,
h4,
h5,
h6 {
    color: $primary;
}
</style>