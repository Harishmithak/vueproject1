<template><div>
   example for keydown: <input type="text"   v-model="inputValue" @keydown.enter="handleEnterKey"><br>
   example for keyup:  <input type="text"  v-model="inputValue2" @keyup.enter="handleEnterKeyup"><br>
   example for keypress:  <input type="text"  v-model="inputValue3" @keypress.enter="handleEnterKeypress"><br>
</div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        inputValue: '',
        inputValue2:'',
        inputValue3:''
      }
    },
    methods: {
      handleEnterKey() {
        alert('you pressed a keydown')

      },
      handleEnterKeyup(){
        alert('you pressed a  keyup')
      },
      handleEnterKeypress()
{
    alert('you pressed a  keypress')
}



      
    }
  };
  </script>
  