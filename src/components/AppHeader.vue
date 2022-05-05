<template>
<header>
  <div class="logo">
    <img src="../assets/img/la-molisana-logo.png" alt="">
  </div>
  <nav>
    <ul>
      <li v-for="(item,index) in links" :key="index" :class="{'selected' : item.active}">{{item.testo}}</li>
    </ul>
  </nav>
</header>
  
    
</template>

<script>
export default {
  name: 'AppHeader',
  data(){
      return{
          links:[
              {
                  testo:'Home',
                  link:'',
                  active:false,
              },
              {
                  testo:'Prodotti',
                  link:'',
                  active:true,
              },
              {
                  testo:'Chi Siamo',
                  link:'',
                  active:false,
              },
               {
                  testo:'Contatti',
                  link:'',
                  active:false,
              },
          ]
      }
  }
  
}
</script>


<style scoped lang="scss">
@import '../style/variables';


.selected{
 background-color: $background;
}

</style>
