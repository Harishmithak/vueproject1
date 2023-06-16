<template>


  <div class="container ">
    <h1 id="p2" >Product Details</h1>
    <div v-for="product in products" >
      <h3  id="p1">{{ ProductDetails}}</h3>
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
  computed:{
    ProductDetails:function(product) {
      if (product.quantity !== 0) {
        return 'The product '+ product.productName+' is available';
      } else {
        return 'The product '+ product.productName +' is not available';
      }
    }
  }
  }
  // methods: {
  //   ProductDetails(product) {
  //     if (product.quantity !== 0) {
  //       return 'The product '+ product.productName+' is available';
  //     } else {
  //       return 'The product '+ product.productName +' is not available';
  //     }
  //   }
  // }




</script>
<style>
#p1{
  font-family: cursive;
    color:rgb(11, 12, 12);
    font-size: 20px;

    background-color: rgb(178, 206, 206);
}
#p2{
  font-family: cursive;
  color: rgb(63, 10, 54);
}
</style>