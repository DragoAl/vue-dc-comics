<template>
  <div id="app">
    <Header />
    <main>
      <Jumbotron/>
      <Products/>

      
    </main>
    <PanelMenu />
    <!-- FOOTER -->
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Jumbotron from './components/Jumbotron.vue'
import Products from './components/Products.vue'
import PanelMenu from './components/PanelMenu.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    Header,
    Jumbotron,
    Products,
    PanelMenu,
    Footer,
    
  }
}
</script>

<style lang="scss"> 
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
  width: 100%;
  margin: 0px auto;
  // font-family: "Greta Sans Condensed Bold","Greta Sans Bold",Arial,sans-serif;
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

</style>
