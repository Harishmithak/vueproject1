<template>
    <div>
      <h2 class="text-dark">Product List</h2>
      <h3>All Product Names:</h3>
      <ul>
        <li v-for="product in products" class="text-white">
          {{ product }}
        </li>
      </ul>
  
      <h3>Product Names with More than One Word:</h3>
      <ul>
        <li v-for="product in morethanoneword" class="text-white">
          {{ product }}
        </li>
      </ul>
  
      <h3>Product Names with Length More than 7 Letters:</h3>
      <ul>
        <li v-for="product in morethan7letters" class="text-white">
          {{ product }}
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        products: [
          "laptop",
          "desktop",
          "tripod",
          "monitor",
          "usb cable",
          "apple ipad",
          "samsung phone"
        ]
      };
    },
    computed: {
        morethanoneword() {
        return this.products.filter(product => product.includes(" "));
      },
      morethan7letters() {
        return this.products.filter(product => product.length > 7);
      }
    }
  };
  </script>
  
  <style >

  
  li {
    font-size: 18px;
    margin-bottom: 5px;
  }
  h3{
    font-family: cursive;
    color:rgb(49, 3, 49);
    font-size: 20px;

    background-color: rgb(178, 206, 206);
  }

  </style>