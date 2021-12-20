<template>
  <div id="app">
    <Header />

  </div>
</template>

<script>
import Header from "./components/Header.vue";


export default {
  name: "App",
  components: {
    Header
  },
};
</script>

<style lang="scss">
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

.container {
  width: 70%;
  margin: auto;
}

img {
  width: 100%;
}

ul {
  list-style-type: none;
}

a {
  text-decoration: none;
  color: inherit;
}
</style>
