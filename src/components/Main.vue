<template>
  <main>
    <div class="container-no-flex">
      <button id="top-button">CURRENT SERIES</button>
      <div class="container-small">
        <Card v-for="(item, index) in cards" :key="index" :carta="item" />
      </div>
      <ButtonPrimary />
    </div>
  </main>
</template>

<script>
import Card from "./Card.vue";
import ButtonPrimary from "./ButtonPrimary.vue";

export default {
  name: "Main",
  components: {
    Card,
    ButtonPrimary,
  },
  props: ["cards"],
};
</script>

<style scoped lang="scss">
@import "../assets/sass/Utilities";
main {
  background-color: black;
  text-align: center;
  position: relative;
}
h2 {
  padding: 30px;
}

button {
  padding: 13px 60px;
  background-color: $my-blue;
  border: 1px solid transparent;
  color: white;
  margin-bottom: 20px;
}

#top-button {
  font-size: 1.2rem;
  position: absolute;
  top: -30px;
  left: 80px;
}
</style>
