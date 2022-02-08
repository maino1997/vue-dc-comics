<template>
  <footer>
    <div class="container">
      <div class="big-col">
        <div class="col">
          <ul>
            <li><h2>DC COMICS</h2></li>
            <li v-for="(link, index) in links" :key="index">
              <a href="#">{{ link.text }}</a>
            </li>
          </ul>
          <ul>
            <li><h2>SHOP</h2></li>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectables</a></li>
          </ul>
        </div>
        <div class="col">
          <ul>
            <li><h2>DC</h2></li>
            <li><a href="#">Terms of Use</a></li>
            <li><a href="#">Privacy Policy</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">Talent Workshop</a></li>
            <li><a href="#">CPSC Certificate</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>
        </div>
        <div class="col">
          <ul>
            <li><h2>SITES</h2></li>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
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

export default {
  name: "FooterTop",
  components: {
    FooterBottom,
  },
  data() {
    return {
      links: [
        {
          text: "CHARACHTERS",
          url: "#",
        },
        {
          text: "COMICS",
          url: "#",
        },
        {
          text: "MOVIES",
          url: "#",
        },
        {
          text: "TV",
          url: "#",
        },
        {
          text: "GAMES",
          url: "#",
        },
        {
          text: "COLLECTIEBILITES",
          url: "#",
        },
        {
          text: "VIDEOS",
          url: "#",
        },
        {
          text: "FANS",
          url: "#",
        },
        {
          text: "NEWS",
          url: "#",
        },
        {
          text: "SHOP",
          url: "#",
        },
      ],
    };
  },
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
  padding-top: 80px;
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  max-height: calc(100% - 260px);
}

#logo-dc {
  height: 400px;
}

ul {
  margin-top: 20px;

  a {
    color: grey;
    font-size: 10px;
  }
}
</style>