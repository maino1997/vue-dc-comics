<template>
  <header>
    <div>
      <img src="../assets/img/dc-logo.png" />
    </div>
    <div>
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
header {
  display: flex;
  justify-content: space-around;
  align-items: center;
  ul {
    display: flex;
    height: 107px;
    li {
      list-style: none;
      display: flex;
      height: 100%;
      margin: 0 10px;
      a {
        height: 107px;
        line-height: 107px;
        font-weight: 600;
        &:hover {
          color: #0c7cec;
          border-bottom: 3px solid #0c7cec;
        }
      }
    }
  }
}
</style>
