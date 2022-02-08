<template>
  <div class="blue-bar">
    <ul>
      <li v-for="(icon, index) in icons" :key="index">
        <img :src="icon.src" alt="" />
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
          src: "../assets/img/buy-comics-digital-comics.png",
        },
        {
          src: "../assets/img/buy-comics-merchandise.png",
        },
        {
          src: "../assets/img/buy-comics-shop-locator.png",
        },
        {
          src: "../assets/img/buy-comics-subscriptions.png",
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
}
</style>