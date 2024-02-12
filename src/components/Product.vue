<template>
  <div class="products-container">
    <ul>
      <li v-for="(productItem, index) in product" :key="index">
        <div class="product">
          <p>Product Name: {{productItem.name}}</p>
          <p>Product Stock: {{ productItem.stock }}</p>
          <p>Product Price: {{ productItem.price }}</p>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  props: ["product"]
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
