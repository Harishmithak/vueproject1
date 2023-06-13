<template>
    <div id="bg">
        <h1>CONTACT US</h1>


        <div>
            <h4 v-if="display">CONTACT NUMBER :{{ contactno }}
                <br>
                ADDRESS :{{ address }}<br>
                EMAIL:{{ email }}
            </h4>
            <button @click="button = !button">SHOW DETAILS</button>
        </div>

    </div>
</template>
  
  
<script>
export default {

    data() {
        return {
            contactno: 9994519917,
            address: '123,mkp colony ,coimbatore-641044',
            email: 'kharishmitha@gmail.com',
            button: true
        }
    },


    computed: {

        display() {
            if (this.button) {
                return false
            }
            else return true
        }
    }
};
</script>
<style>
#bg {
    background-color: lightseagreen;
}

h1 {
    color: darkslateblue;
}
h4{
    color:crimson;
}
</style>