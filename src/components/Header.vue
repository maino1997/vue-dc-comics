<template>
  <header>
    <div>
      <img src="../assets/img/dc-logo.png" />
    </div>
    <div class="list-cont">
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a href="#">{{ link.text }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  components: {},
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
@import "Utilities";
header {
  display: flex;
  justify-content: space-around;
  align-items: center;
  .list-cont {
    height: 100%;
    ul {
      display: flex;
      height: 127px;
      li {
        list-style: none;
        display: flex;
        height: 100%;
        margin: 0 10px;
        a {
          height: 100%;
          line-height: 127px;
          font-weight: 600;
          &:hover {
            color: $my-blue;
            border-bottom: 3px solid $my-blue;
          }
        }
      }
    }
  }
}

img {
  padding: 10px 0;
}
</style>
