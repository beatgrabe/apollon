<template>
  <svg
    width="100"
    height="100"
    viewBox="0 0 42 42"
    class="donut"
  >
    <circle
      class="donut-hole"
      cx="21"
      cy="21"
      r="15.91549430918954"
      fill="#fff"
    />
    <circle
      class="donut-ring"
      cx="21"
      cy="21"
      r="15.91549430918954"
      fill="transparent"
      stroke="silver"
      stroke-width="5"
    />
    <circle
      class="donut-segment1"
      cx="21"
      cy="21"
      r="15.91549430918954"
      fill="transparent"
      stroke="deepskyblue"
      stroke-width="5"
      stroke-dasharray="40 60"
      stroke-dashoffset="25"
    />
    <circle
      class="donut-segment2"
      cx="21"
      cy="21"
      r="15.91549430918954"
      fill="transparent"
      stroke="dodgerblue"
      stroke-width="5"
      stroke-dasharray="20 80"
      stroke-dashoffset="85"
    />
    <circle
      class="donut-segment3"
      cx="21"
      cy="21"
      r="15.91549430918954"
      fill="transparent"
      stroke="aliceblue"
      stroke-width="5"
      stroke-dasharray="30 70"
      stroke-dashoffset="65"
    />
  </svg>
</template>

<script>
export default {
  name: 'Doughnut'
}
</script>

<style lang="scss" scoped>

</style>
