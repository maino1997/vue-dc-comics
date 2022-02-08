<template>
  <div class="footer-bottom">
    <div class="container">
      <!-- <div class="content"> -->
      <div class="left">
        <a href="#">Sign Up Now</a>
      </div>
      <div class="right">
        <ul>
          <li><h3>FOLLOW US</h3></li>
          <li>
            <img src="../assets/img/footer-facebook.png" alt="facebook" />
          </li>
          <li><img src="../assets/img/footer-twitter.png" alt="facebook" /></li>
          <li><img src="../assets/img/footer-youtube.png" alt="facebook" /></li>
          <li>
            <img src="../assets/img/footer-pinterest.png" alt="facebook" />
          </li>
          <li>
            <img src="../assets/img/footer-periscope.png" alt="facebook" />
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
};
</script>

<style scoped lang="scss">
.footer-bottom {
  height: 100px;
  background-color: rgb(34, 32, 32);
  position: fixed;
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
  display: flex;
  justify-content: center;
  align-items: center;
  a {
    border: 2px solid #0c7cec;
    color: white;
    padding: 15px 5px 15px 5px;
  }
}

.right {
  h3 {
    color: #0c7cec;
  }
  ul {
    display: flex;
    li {
      margin: 10px;
    }
  }
}
</style>