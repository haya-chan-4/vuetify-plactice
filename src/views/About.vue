<template>
  <v-container id="container-full">
    <v-layout>
      <v-flex xs12>
        <v-img src="https://www.symph.co/static/img/banner-illus.svg"></v-img>
      </v-flex>
    </v-layout>

    <v-layout text-center mt-5 px-3 py-3 id="about">
      <v-flex xs12>
        <span class="display-2 font-weight-bold">About Me</span>
      </v-flex>
    </v-layout>

    <v-layout mt-3 px-5 class="text-center" row wrap>
      <v-flex xs12>
        <v-avatar size="250" color="blue lighten-4">
          <img
            src="../assets/logo.png"
            alt="avatar"
          >
        </v-avatar>
        <p class="headline font-weight mt-2">HAYATA TAKE</p>
        <p
          class="title font-weight-thin mt-3"
        >Hello I'm a Full Stack Web Developer and iOS Developer from Philippines. Have 5 years work experience in IT Industry.</p>
      </v-flex>
    </v-layout>

    <v-layout text-center mt-10 px-3 py-3 primary row wrap>
      <v-flex xs12>
        <span class="display-2 font-weight-bold white--text" id="skills">Skill Sets</span>
      </v-flex>
    </v-layout>
    <v-layout text-center px-3 py-3 primary row wrap>
      <v-flex lg4 sm12 xs12>
        <v-avatar size="150" color="grey lighten-4">
          <img src="../assets/logo.svg" alt="avatar">
        </v-avatar>
        <p class="subheading font-weight mt-2 white--text">Vuetify</p>
      </v-flex>
      <v-flex lg4 sm12 xs12>
        <v-avatar size="150" color="grey lighten-4">
          <img src="https://cdn.auth0.com/blog/react-js/react.png" alt="avatar">
        </v-avatar>
        <p class="subheading font-weight mt-2 white--text">React.js</p>
      </v-flex>
      <v-flex lg4 sm12 xs12>
        <v-avatar size="150" color="grey lighten-4">
          <img
            src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/cf/Angular_full_color_logo.svg/1200px-Angular_full_color_logo.svg.png"
            alt="avatar"
          >
        </v-avatar>
        <p class="subheading font-weight mt-2 white--text">Angular 7</p>
      </v-flex>
    </v-layout>
    <v-layout text-center px-3 py-3 primary row wrap>
      <v-flex lg4 sm12 xs12>
        <v-avatar size="150" color="grey lighten-4">
          <img src="../assets/logo.png" alt="avatar">
        </v-avatar>
        <p class="subheading font-weight mt-2 white--text">Vue.js</p>
      </v-flex>
      <v-flex lg4 sm12 xs12>
        <v-avatar size="150" color="grey lighten-4">
          <img
            src="https://cdn.freebiesupply.com/logos/large/2x/mysql-6-logo-png-transparent.png"
            alt="avatar"
          >
        </v-avatar>
        <p class="subheading font-weight mt-2 white--text">MySQL</p>
      </v-flex>
      <v-flex lg4 sm12 xs12>
        <v-avatar size="150" color="grey lighten-4">
          <img src="https://go.neo4j.com/rs/710-RRC-335/images/neo4j_logo_globe.png" alt="avatar">
        </v-avatar>
        <p class="subheading font-weight mt-2 white--text">Neo4j</p>
      </v-flex>
    </v-layout>
  </v-container>
</template>