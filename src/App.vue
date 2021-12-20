<template>
  <div id="app">
    <Header />

    <main>
      <MainContent />
    </main>

    <PreFooter />

    <footer>
      <FooterLinkList />
      <FooterSocials />
    </footer>

  </div>
</template>

<script>
import Header from "./components/Header.vue";
import MainContent from "./components/MainContent.vue";
import PreFooter from "./components/PreFooter.vue";
import FooterLinkList from "./components/FooterLinkList.vue";
import FooterSocials from "./components/FooterSocials.vue";


export default {
  name: "App",
  components: {
    Header,
    MainContent,
    PreFooter,
    FooterLinkList,
    FooterSocials
  },
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@500&display=swap');

// RESET
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

// COMMON
#app {
  font-family: 'Oswald', sans-serif;
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

// MAIN
main {
  background-color: black;
  color: white;
  padding: 50px 0;
}
</style>
