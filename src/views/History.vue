<template>
  <v-container>
    <h2>{{ $t("historyTitle") }}</h2>
    <p> {{ $t("historyDescription") }}
    </p>
  </v-container>
</template>

<script>

// watch: {
//   input: function () {
//     if (isLocalStorage() /* function to detect if localstorage is supported*/) {
//       localStorage.setItem('storedData', this.input)
//     }
//   }
// }
// json.parse(localStorage.getItem('history'));
// app.input = localStorage.getItem('history');
// console.log('history')

export default {
name: "History"
}
</script>

<style scoped>

</style>
