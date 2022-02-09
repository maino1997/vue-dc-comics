<template>
  <div class="footer-bottom">
    <div class="container">
      <!-- <div class="content"> -->
      <div class="left flex-center">
        <a href="#">Sign Up Now</a>
      </div>
      <div class="right">
        <ul>
          <li><h3>FOLLOW US</h3></li>
          <li v-for="(url, index) in urls" :key="index">
            <img :src="url.source" alt="icon" />
          </li>
        </ul>
      </div>
    </div>
    <!-- </div> -->
  </div>
</template>

<script>
export default {
  name: "FooterBottom",
  data() {
    return {
      urls: [
        {
          source: require("../assets/img/footer-facebook.png"),
        },
        {
          source: require("../assets/img/footer-twitter.png"),
        },
        {
          source: require("../assets/img/footer-youtube.png"),
        },
        {
          source: require("../assets/img/footer-pinterest.png"),
        },
        {
          source: require("../assets/img/footer-periscope.png"),
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "Utilities";
.footer-bottom {
  height: 80px;
  background-color: rgb(34, 32, 32);
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  display: flex;
  align-items: center;
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.left {
  a {
    border: 2px solid #0c7cec;
    color: white;
    padding: 15px 5px 15px 5px;
  }
}

.right {
  h3 {
    color: $my-blue;
  }
  ul {
    display: flex;
    li {
      margin: 10px;
    }
  }
}
</style>