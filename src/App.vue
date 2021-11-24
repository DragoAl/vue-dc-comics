<template>
  <div id="app">
    <Header />
    <main>
      <section>
        CONTENT GOES HERE
      </section>
      
    </main>
    <PanelMenu />
    <!-- FOOTER -->
    <Footer/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import PanelMenu from './components/PanelMenu.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    PanelMenu,
    Footer
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

main {
  background-color: #1c1c1c ;
  height: 100px;
  color: white;
  vertical-align: middle;
  line-height: 100px;

  section {
    width: 75%;
    margin: 0 auto;
  }
  

}
</style>
