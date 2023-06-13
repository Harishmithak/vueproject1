
<!-- assignment 1 -->

<!-- <template>

  <div class="container">
    <h5 class="fw-bolder h1">EMPLOYEE DETAILS</h5>

    <h4>The employee code is :{{ employeecode }}</h4>

    <h4>The employee name is :{{ employeename }}</h4>

    <h4>The employee date of joining is :{{ doj }}</h4>

    <h4>The employee department is :{{ department }}</h4>

    <h4>The employee designation is :{{ designation }}</h4>

    <h4>The employee salary is :{{ salary }}</h4>

    <h4>The employee experience is :{{ experience }}years</h4>


    <h4>The employee bonus is :{{ bonus() }}</h4>

    <h4>The employee total salary is :{{ totalsalary() }}</h4>

  </div>

  <product></product>
</template>


<script>
export default {
  data() {
    return {
      employeecode: 101,
      employeename: 'Harishmitha',
      doj: '12/1/2020',
      department: 'HR',
      designation: 'developer',
      salary: 20000,
      experience: 1,

    }
  },
  methods: {
    bonus() {
      var bonus1 = (this.experience > 5 ? '5000' : (this.experience > 2 ? '3000' : '1500'))
      return bonus1

    },
    totalsalary() {
      var totalsalary1 = parseInt(this.bonus()) + parseInt(this.salary);
      return totalsalary1
    }

  }

}

import product from './components/product.vue'
</script>







<style>
body {
  background-color: rgb(226, 189, 212);
}

.h1 {
  color: blue;
}
h4{
  color: rgb(34, 19, 31);
}
</style> -->



<!-- ASSIGNMENT 2 -->

<template>

 <!-- <product> </product> -->
<array> </array>
<!-- <contact> </contact> -->
</template>


<script>
import product from './components/product.vue'
import array from './components/array.vue'
import contact from './components/contact.vue'

export default{
  
  components: {
    product,
    array,
    contact
  
  }}

</script>

<style>


</style>