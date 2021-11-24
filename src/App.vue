<template>
  <div id="app">
    <Header />
    <main>
      CONTENT GOES HERE
      <!--COMPONENTE BLU AGGIUNTIVO AGGIUNGERE AL MAIN  -->
      <PanelMenu />
    </main>
    <!-- FOOTER -->
  </div>
</template>

<script>
import Header from './components/Header.vue'
import PanelMenu from './components/PanelMenu.vue'

export default {
  name: 'App',
  components: {
    Header,
    PanelMenu
  }
}
</script>

<style lang="scss">
#app {
  // font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 60%;
  margin: 30px auto;
  font-family: "Greta Sans Condensed Bold","Greta Sans Bold",Arial,sans-serif;}
</style>
