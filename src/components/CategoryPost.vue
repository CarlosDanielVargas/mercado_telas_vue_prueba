<script>
import axios from 'axios';
export default {
  data(){
    return {
      name: ''
    };
  },
  methods: {
    onCreateCategory(){
      const category = {
        category: {
          name: this.name
        }
      };
      axios.post('http://localhost:3000/categories', category).then(response => {
        console.log(response);
      });
    }
  }
}

</script>

<template>
<div>
    <h1>Category Category</h1>
    <form @submit.prevent="onCreateCategory">
        <label for="category">Category</label>
        <input type="text" id="category" name="category" v-model="name">
        <button type="submit">Submit</button>
    </form>
</div>
</template>

<style scoped>

</style>