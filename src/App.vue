<template>
  <v-app>
    <v-main app>
      <router-view />
    </v-main>

    <v-bottom-navigation
      app
      grow
    >
      <v-btn
        height="56"
        to="home"
      >
        <v-icon color="primary">
          mdi-domain
        </v-icon>
      </v-btn>

      <v-btn
        height="56"
        to="search"
      >
        <v-icon color="primary">
          mdi-magnify
        </v-icon>
      </v-btn>
    </v-bottom-navigation>
  </v-app>
</template>

<script>
export default {
  name: 'App'
}
</script>
