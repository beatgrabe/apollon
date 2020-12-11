<template>
  <div>
    <v-app-bar
      dense
      flat
    >
      <div class="title">
        Home
      </div>

      <v-spacer />

      <v-btn
        icon
        small
      >
        <v-icon>mdi-dots-vertical </v-icon>
      </v-btn>
    </v-app-bar>

    <div class="home">
      <v-list>
        <v-subheader>Overview</v-subheader>
        <v-list-item
          v-for="item in overviewItems"
          :key="item.text"
        >
          <v-list-item-content>
            <v-list-item-title v-text="item.text" />
          </v-list-item-content>
        </v-list-item>

        <v-spacer />

        <v-subheader>Favorits</v-subheader>
        <v-list-item
          v-for="item in favorits"
          :key="item.text"
        >
          <v-list-item-content>
            <v-list-item-title v-text="item.text" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',

  data: () => ({
    overviewItems: [
      {
        text: 'WARNING'
      },
      {
        text: 'STOP'
      }
    ],
    favorits: [
      {
        text: 'Foo'
      },
      {
        text: 'Bar'
      }
    ]
  })
}
</script>
