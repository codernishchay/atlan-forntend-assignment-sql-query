<template>
  <v-app-bar
    :clipped-left="clipped"
    fixed
    dense
    color="purple"
    app
  >
    <v-toolbar-title class="mr-5 white--text">
      {{ title }}
    </v-toolbar-title>
    <span class="white--text">SQL Editor challenge</span>
    <v-spacer/>
    <v-btn
      icon
      x-large
      :link="true"
      href="https://github.com/satyamsingh-sg/atlan-forntend-assignment-sql-query.git"
    >
      <v-icon>mdi-github</v-icon>
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {
  name: "AppBar",
  data () {
    return {
      clipped: true,
      title: 'Atlan',
      mini: false,
    }
  },
}
</script>
