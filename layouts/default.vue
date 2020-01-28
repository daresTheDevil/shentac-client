<template>
  <v-app>
    <!-- <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer> -->
    <v-app-bar
      :clipped-left="clipped"
      fixed
      app
      color="blue-grey lighten-5"
      elevate-on-scroll
    >
      <!-- <v-app-bar-nav-icon @click.stop="drawer = !drawer" /> -->
      <!-- 
      <v-btn @click.stop="miniVariant = !miniVariant" icon>
        <v-icon>mdi-{{ `chevron-${miniVariant ? 'right' : 'left'}` }}</v-icon>
      </v-btn>
      <v-btn @click.stop="clipped = !clipped" icon>
        <v-icon>mdi-application</v-icon>
      </v-btn>
      <v-btn @click.stop="fixed = !fixed" icon>
        <v-icon>mdi-minus</v-icon>
      </v-btn> -->

      <v-toolbar-title>Shenandoah Tactical</v-toolbar-title>
      <v-spacer />

      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn text>Home</v-btn>
        <v-btn text>Calendar</v-btn>
        <v-btn text disabled>Register</v-btn>
      </v-toolbar-items>
      <v-btn icon large class="hidden-sm-and-down">
        <v-icon large color="light-blue darken-2">mdi-facebook</v-icon>
      </v-btn>
      <v-btn icon large class="hidden-sm-and-down">
        <v-icon large color="red darken-2">mdi-instagram</v-icon>
      </v-btn>

      <v-btn
        @click.stop="rightDrawer = !rightDrawer"
        icon
        class="hidden-sm-and-up"
      >
        <v-icon>mdi-menu</v-icon>
      </v-btn>
    </v-app-bar>
    <v-content class="blue-grey lighten-5">
      <nuxt />
    </v-content>
    <v-navigation-drawer v-model="rightDrawer" :right="right" temporary fixed>
      <v-list>
        <v-subheader>Social</v-subheader>
        <v-list-item>
          <v-list-item-action class="mr-4">
            <v-icon large color="light-blue darken-2">
              mdi-facebook
            </v-icon>
          </v-list-item-action>
          <v-list-item-title>Connect on Facebook</v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-action class="mr-4">
            <v-icon large color="red darken-2">
              mdi-instagram
            </v-icon>
          </v-list-item-action>
          <v-list-item-title>Connect on Instagram</v-list-item-title>
        </v-list-item>
      </v-list>
      <v-divider />
      <v-list>
        <v-subheader>Links</v-subheader>
        <v-list-item>
          <v-list-item-title>Our Classes</v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-title>Our Services</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <!-- <v-footer :fixed="fixed" app>
      <span>&copy; 2019</span>
    </v-footer> -->
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
