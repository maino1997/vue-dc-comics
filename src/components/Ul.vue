<template>
  <div>
    <li v-for="(link, index) in firstUl" :key="index">
      <a href="#">{{ link.text }}</a>
    </li>
  </div>
</template>

<script>
export default {
  name: "Ul",
  props: ["firstUl"],
};
</script>

<style>
</style>