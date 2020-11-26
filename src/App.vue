<template>
  <v-app>
    <SideNav message="Navigation Lists" />
    <Header @toggle="open" />

    <v-main>
      <router-view  />
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

  // props: ['drawer'],

  data(){
    return{
      // drawer: null,
    }
  },
  methods: {
    open(drawer) {
      console.log(drawer)
      console.log('受け取りました')

      if(drawer) {
        console.log(drawer)
      }
    }
  }
};
</script>
