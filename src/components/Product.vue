<template>
  <div class="products-container">
    <ul>
      <li v-for="(product, index) in products" :key="index">
        <div class="product">
          <p>Product Name: {{ product.name }}</p>
          <p>Product Stock: {{ product.stock }}</p>
          <p>Product Price: {{ product.price }}</p>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  props: ["product"],
  data() {
    const products = this.$props.product;
    return { products };
  },
};
</script>
<style>
.products-container {
  display: flex;
  justify-content: center;
}
.product {
  display: flex;
  justify-content: space-around;
}
</style>
