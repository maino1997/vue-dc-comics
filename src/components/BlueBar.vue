<template>
  <div class="blue-bar">
    <ul>
      <li v-for="(icon, index) in icons" :key="index">
        <img :src="icon.src" alt="ciao" />
        <span>{{ icon.text }}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "BlueBar",
  data() {
    return {
      icons: [
        {
          src: require("../assets/img/buy-comics-digital-comics.png"),
          text: "DITIGAL COMICS",
        },
        {
          src: require("../assets/img/buy-comics-merchandise.png"),
          text: "DC MERCHANDISE",
        },
        {
          src: require("../assets/img/buy-comics-shop-locator.png"),
          text: "SUBSCRIPTION",
        },
        {
          src: require("../assets/img/buy-comics-subscriptions.png"),
          text: "COMIC SHOP LOCATOR",
        },
        {
          src: require("../assets/img/buy-dc-power-visa.svg"),
          text: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "Utilities";
.blue-bar {
  position: fixed;
  left: 0;
  right: 0;
  top: 27%;
  height: 100px;
  background-color: $my-blue;
}

ul {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  li {
    display: flex;
    align-items: center;
    margin: 0 20px;
    span {
      color: white;
      margin: 0 10px;
      font-size: 0.8rem;
    }
  }
}

img {
  height: 55px;
}
</style>