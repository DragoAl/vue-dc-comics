<template>
  <div id="app">
    <Header />

    <main>
      <Jumbotron/>
      <Products/>
      <PanelMenu />
    </main>

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
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  width: 100%;
  margin: 0px auto;
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

</style>
