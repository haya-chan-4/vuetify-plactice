<template>
  <v-navigation-drawer color="#eefe" clipped app>
      <v-container>
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title class="title grey--text text--darken-2">
              {{message}}
              {{drawer}}
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-divider></v-divider>

        <v-list nav dense>
          <v-list-group
          v-for="nav_list in nav_lists"
          :key="nav_list.name"
          :prepend-icon="nav_list.icon"
          no-action
          :append-icon="nav_list.lists ? undefined : ''">
            <template v-slot:activator>
              <v-list-item-content>
                <v-list-item-title>{{ nav_list.name }}</v-list-item-title>
              </v-list-item-content>
            </template>
            <v-list-item v-for="list in nav_list.lists" :key="list.name" :to="list.link">
              <v-list-item-content>
                <v-list-item-title>{{ list }}</v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list-group>
        </v-list>
      </v-container>
    </v-navigation-drawer>
</template>

<script>


export default {
  components: {

  },

  props: {
    drawer: {
      type: String,
      required: null,
    },
    message: {
      type: String
    }
  },

  data() {
    return {
      // drawer: null,
      nav_lists:[
          {
            name: 'Getting Started',
            icon: 'mdi-speedometer',
            lists:['Quick Start','Pre-made layouts']
          },
          {
            name: 'Customization',
            icon: 'mdi-cogs'
          },
          {
            name: 'Styles & animations',
            icon: 'mdi-palette',
            lists:['Colors','Content','Display']
          },
          {
            name: 'UI Components',
            icon: 'mdi-view-dashboard',
            lists:['API explorer','Alerts']
          },
          {
            name: 'Directives',
            icon: 'mdi-function'
          },
          {
            name: 'Preminum themes',
            icon: 'mdi-vuetify'
          },
        ]
    }
  },
  methods: {

  }
}
</script>