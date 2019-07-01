<template>
  <div>
    <input type="text" v-model="simple">
    <p>{{simple}}</p>
    <button v-on:click="enter">ENTER</button>
  </div>
</template>

<script>
    export default {
        name: "input",
      data:{

            simple:''


      },
      methods:{
          enter:function () {
                this.simple='';
          }
      }
    }
</script>

<style scoped>

</style>
