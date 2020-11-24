<template>
  <v-app>
    <SideNav />
    <Header />

    <v-main>
      <router-view />
    </v-main>

    <Footer />
  </v-app>
</template>

<script>
import Header from "./components/Header.vue"
import SideNav from "./components/SideNav.vue"
import Footer from "./components/Footer.vue"


export default {
  name: 'App',

  components: {
    Header,
    SideNav,
    Footer
  },

  data(){
    return{
      data(){
        return {
          drawer: null,
        }
      }
    }
  }
};
</script>
