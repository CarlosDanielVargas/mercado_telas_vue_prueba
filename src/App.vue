<script setup>
import CategoryPost from "@/components/CategoryPost.vue";

</script>
import CategoryPost from "./components/CategoryPost.vue";
export default {
  name: 'App',
  components: {
    CategoryPost,
  }
}
<script>

</script>

<template>
<div id="app">
    <header>
      <div class="wrapper">
        <CategoryPost />
      </div>
    </header>
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
}


@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }


  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
