<template>
    <div>
        <Product :product="productList"/>
    </div>
</template>
<script>
import Product from './Product.vue';
export default({
    components:{
        Product
    },
    data() {
      return {
        productList:[
            {name:'Pencil',stock:10,price:2},
            {name:'Notebook',stock:15,price:5},
            {name:'Book',stock:20,price:6}
        ]
      }
        
    }
})
</script>