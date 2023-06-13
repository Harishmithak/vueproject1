<template>


  <div>
    <h1>Product Details</h1>
    <div v-for="product in products" >
      <h3>{{ ProductDetails(product) }}</h3>
    </div>
  </div>
</template>



<script>
export default {
  data() {
    return {
      products: [
        {
          productName: 'Mobile',
          quantity: 1
        
        },
        {
          productName: 'Laptop',
          quantity: 0
        
        },
        {
          productName: 'camera',
          quantity: 1
        
        },
        {
          productName: 'tripod',
          quantity: 0
        
        }
      ]
    };
  },
  methods: {
    ProductDetails(product) {
      if (product.quantity !== 0) {
        return 'The product name is '+ product.productName;
      } else {
        return 'The product '+ product.productName +' is not available';
      }
    }
  }
};


</script>