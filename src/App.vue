<template>
  <div id="app">
    <AppHeader />

    <main>
      <AppJumbotron/>
      <Products/>
      <PanelMenu />
    </main>

    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppJumbotron from './components/AppJumbotron.vue'
import Products from './components/Products.vue'
import PanelMenu from './components/PanelMenu.vue'
import AppFooter from './components/AppFooter.vue'


export default {
  name: 'App',
  components: {
    AppHeader,
    AppJumbotron,
    Products,
    PanelMenu,
    AppFooter,
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
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

</style>
