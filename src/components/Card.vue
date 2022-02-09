<template>
  <figure class="card-class">
    <img :src="carta.thumb" alt="carta.series " />
    <figcaption>{{ carta.series }}</figcaption>
  </figure>
</template>

<script>
export default {
  name: "Card",
  props: ["carta"],
};
</script>

<style scoped lang='scss'>
.card-class {
  width: calc(100% / 6 - 10px);
  padding: 50px 10px;
}

figcaption {
  color: white;
}

img {
  width: 100%;
  height: 170px;
}
</style>