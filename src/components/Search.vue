<template>
  <div class="search-wrap">
    <input type="text" class="search-field" v-model="userSearch" placeholder="search"/>
    
  </div>
</template>

<script>
export default {
  name: "Search",
  props: ["products"],  
};
</script>

<style scoped>

</style>
