<template>
  <div>
    <Header />
    <Main />
    <FooterTop />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import FooterTop from "./components/FooterTop.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    FooterTop,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Segoe UI", "Open Sans", Helvetica, sans-serif;
}

.container {
  max-width: 1200px;
  width: 100%;
  display: flex;
  margin: auto;
}

ul {
  list-style: none;
}

h2 {
  color: white;
}

a {
  text-decoration: none;
  color: black;
  cursor: pointer;
}
</style>
