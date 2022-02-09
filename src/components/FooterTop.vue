<template>
  <footer>
    <Blue-bar />
    <div class="container">
      <div class="big-col">
        <div class="col">
          <ul>
            <li><h2>DC COMICS</h2></li>
            <li v-for="(link, index) in firstUl" :key="index">
              <a href="link.url">{{ link.text }}</a>
            </li>
          </ul>
          <ul>
            <li><h2>SHOP</h2></li>
            <li v-for="(link, index) in secondUl" :key="index">
              <a href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col">
          <ul>
            <li><h2>DC</h2></li>
            <li v-for="(link, index) in thirdUl" :key="index">
              <a href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col">
          <ul>
            <li><h2>SITES</h2></li>
            <li v-for="(link, index) in fourthUl" :key="index">
              <a href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
      </div>
      <div class="big-col">
        <img src="../assets/img/dc-logo-bg.png" alt="logo-dc" id="logo-dc" />
      </div>
    </div>

    <FooterBottom />
  </footer>
</template>

<script>
import FooterBottom from "./FooterBottom.vue";
import BlueBar from "./BlueBar.vue";

export default {
  name: "FooterTop",
  components: {
    FooterBottom,
    BlueBar,
  },
  props: ["firstUl", "secondUl", "thirdUl", "fourthUl"],
};
</script>

<style scoped lang="scss">
.big-col {
  width: 50%;
  display: flex;
}

.col {
  width: calc(100% / 3);
}

footer {
  position: relative;
  padding-top: 90px;
  padding-bottom: 65px;
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

#logo-dc {
  height: 420px;
}

ul {
  margin-top: 20px;

  a {
    color: rgb(180, 161, 161);
    font-size: 13px;
  }
}
</style>