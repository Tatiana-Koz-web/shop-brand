<template>
  <div class="grid-container">
    <Search :products="products"/>
    <div class="grid-wrap">
      <ProductsGridItem
        v-for="product in products"
        :key="product.id"
        :product="product"
      />
    </div>
  </div>
</template>

<script>
import ProductsGridItem from "./ProductsGridItem";
import Search from "./Search.vue";
export default {
  name: "ProductsGrid",
  props: ["products"],
  components: {
    ProductsGridItem,
    Search,
  },
};
</script>

<style scoped>
.grid-wrap {
  display: flex;  
  flex-wrap: wrap;
  justify-content: space-between;
  margin-top: 16px;
}
</style>
