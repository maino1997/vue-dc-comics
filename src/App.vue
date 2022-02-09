<template>
  <div>
    <Header />
    <Jumbodron />
    <Main :cards="cards" />
    <FooterTop
      :firstUl="ulLists.firstUl"
      :secondUl="ulLists.secondUl"
      :thirdUl="ulLists.thirdUl"
      :fourthUl="ulLists.fourthUl"
    />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import FooterTop from "./components/FooterTop.vue";
import Jumbodron from "./components/Jumbodron.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    FooterTop,
    Jumbodron,
  },
  data() {
    return {
      cards: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
      ulLists: {
        firstUl: [
          {
            text: "Characters",
            url: "#",
          },
          {
            text: "Comics",
            url: "#",
          },
          {
            text: "Movies",
            url: "#",
          },
          {
            text: "Tv",
            url: "#",
          },
          {
            text: "Games",
            url: "#",
          },
          {
            text: "Collectabilites",
            url: "#",
          },
          {
            text: "Videos",
            url: "#",
          },
          {
            text: "Fans",
            url: "#",
          },
          {
            text: "News",
            url: "#",
          },
          {
            text: "Shop",
            url: "#",
          },
        ],
        secondUl: [
          {
            text: "Shop DC",
            url: "#",
          },
          {
            text: "Shop DC Collectables",
            url: "#",
          },
        ],
        thirdUl: [
          {
            text: "Terms of Use",
            url: "#",
          },
          {
            text: "Privacy Policy",
            url: "#",
          },
          {
            text: "Ad Choices",
            url: "#",
          },
          {
            text: "Advertising",
            url: "#",
          },
          {
            text: "Jobs",
            url: "#",
          },
          {
            text: "Subscriptions",
            url: "#",
          },
          {
            text: "Talent Workshop",
            url: "#",
          },
          {
            text: "CPSC Certificate",
            url: "#",
          },
          {
            text: "Ratings",
            url: "#",
          },
          {
            text: "Shop Help",
            url: "#",
          },
          {
            text: "Contact Us",
            url: "#",
          },
        ],
        fourthUl: [
          {
            text: "DC",
            url: "#",
          },
          {
            text: "MAD Magazine",
            url: "#",
          },
          {
            text: "DC Kids",
            url: "#",
          },
          {
            text: "DC Universe",
            url: "#",
          },
          {
            text: "DC Power Visa",
            url: "#",
          },
        ],
      },
    };
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

.container-small {
  max-width: 1000px;
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  margin: auto;
  justify-content: center;
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
