<template>
  <v-banner
    v-if="showResult"
    single-line
    sticky
  >
    <span class="purple--text mr-3 caption">success</span>
    <span class="white--text caption">({{ selectedQuery.queryResult.length }} rows)0.189 seconds</span>
    <v-spacer/>
  </v-banner>
</template>

<script>
import { mapState } from 'vuex'
export default {
  name: "Banner",
  computed: {
    ...mapState([
      'selectedQuery',
      'showResult'
    ])
  },
}
</script>
