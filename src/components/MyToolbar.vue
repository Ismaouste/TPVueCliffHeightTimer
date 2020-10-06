<template>
  <div>
    <v-app-bar dark color="deep-purple" clipped-left app>
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title @click="goHome" class="white--text">Cliff height timer</v-toolbar-title>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name: 'myToolbar',
  data: function () {
    return {
      drawer: false
    }
  },
  methods: {
    goHome () {
      this.$router.replace('/')
    }
  }
}
</script>

