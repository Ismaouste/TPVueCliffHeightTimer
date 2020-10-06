<template>
  <v-container>
    <h2>{{ $t("historyTitle") }}</h2>
    <p> {{ $t("historyDescription") }}
    </p>
    <div>
      <ul v-for="key in history" :key="key.time">
        <li> time : {{key.time}}</li>
        <li> m : {{key.m}}</li>
        <li> ft : {{key.ft}}</li>

      </ul>
    </div>
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
name: "History",
  data: function () {
    return {
      history: JSON.parse(localStorage.getItem("history"))
    }
  }
}
</script>

<style scoped>

</style>
