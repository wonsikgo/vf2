<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
      <SiteTitle></SiteTitle>
      <v-toolbar-title>Page title</v-toolbar-title>
      <v-spacer></v-spacer>

      <v-btn icon to="/about">
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
    </v-app-bar>
    <v-content>
      <router-view></router-view>
    </v-content>
    <SiteFooter></SiteFooter>
  </v-app>
</template>

<script>
import SiteTitle from '@/views/site/Title'
import SiteFooter from '@/views/site/Footer'
export default {
  name: 'App',
  components: {
    SiteTitle,
    SiteFooter
  }
}
</script>
