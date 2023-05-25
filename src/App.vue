<template>
  <div>

  </div>

</template>

<script>
import axios from "axios";
export default {
  name: "App",

  async mounted() {
    let results = await axios.get("http://0.0.0.0:3000/categories");
    console.log(results);
  }
};
</script>