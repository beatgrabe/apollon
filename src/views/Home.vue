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

    <div class="chart">
      <doughnut />
      <ul class="list">
        <li class="cat1">
          8 lorem
        </li>
        <li class="cat2">
          4 ipsum
        </li>
        <li class="cat3">
          2 dolor
        </li>
        <li class="cat4">
          1 sum
        </li>
      </ul>
    </div>

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
import Doughnut from '../components/Doughnut'

export default {
  name: 'Home',

  components: {
    Doughnut
  },

  data: () => {
    return {
      overviewItems: [
        { text: 'WARNING' },
        { text: 'STOP' }
      ],
      favorits: [
        { text: 'Foo' },
        { text: 'Bar' }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.chart {
  align-items: center;
  display: flex;
  padding: 8px;

  .cat1::marker {
    color: deepskyblue;
  }

  .cat2::marker {
    color: dodgerblue;
  }

  .cat3::marker {
    color: aliceblue;
  }

  .cat4::marker {
    color: silver;
  }

  .list {
    font-size: 14px;
  }
}
</style>
