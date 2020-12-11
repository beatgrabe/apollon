<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
      dense
    >
      <div class="title">
        Apollon
      </div>

      <v-spacer />

      <v-btn
        icon
        small
      >
        <v-icon>mdi-dots-vertical </v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>

    <v-bottom-navigation>
      <v-btn to="home">
        <v-icon color="primary">
          mdi-view-headline
        </v-icon>
      </v-btn>

      <v-btn to="search">
        <v-icon color="primary">
          mdi-magnify
        </v-icon>
      </v-btn>

      <v-btn>
        <v-icon color="primary">
          mdi-cog
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
