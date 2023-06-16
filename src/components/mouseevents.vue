<template>
    <div>
      <div v-on:mouseenter="handleMouseEnter" @mouseleave="handleMouseLeave" class="box">
        <p>{{ message }}</p>
      </div>
    
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        message: "Hover over the box",
      };
    },
    methods: {
      handleMouseEnter() {
        this.message = "Mouse entered the box";
      },
      handleMouseLeave() {
        this.message = "Mouse left the box";
      }
      
    },
  };
  </script>
  
  <style>
  .box {
    width: 200px;
    height: 200px;
    background-color: lightblue;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  </style>
  