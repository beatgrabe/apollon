<template>
  <div class="search">
    <h1>Search</h1>
    <v-text-field
      label="Go to"
      prepend-inner-icon="mdi-magnify"
      solo
    />
    <v-list>
      <v-subheader>Recent</v-subheader>
      <v-list-item
        v-for="item in recents"
        :key="item.text"
      >
        <v-list-item-content>
          <v-list-item-title v-text="item.text" />
        </v-list-item-content>
      </v-list-item>

      <v-divider />
      <v-subheader>Areas</v-subheader>
      <v-list-item
        v-for="item in areas"
        :key="item.text"
      >
        <v-list-item-content>
          <v-list-item-title v-text="item.text" />
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </div>
</template>

<script>
export default {
  name: 'Search',

  data: () => ({
    recents: [
      {
        text: 'Foo'
      },
      {
        text: 'Bar'
      }
    ],
    areas: [
      {
        text: 'Foos'
      },
      {
        text: 'Bars'
      }
    ]
  })
}
</script>

<style lang="scss" scoped>
.search {
  padding: 8px
}
</style>
