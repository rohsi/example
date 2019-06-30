<template>
  <div>
    <input type="text" v-model="simple">
    <p>{{simple}}</p>
  </div>
</template>

<script>
    export default {
        name: "input",
      data(){
          return{
            simple:''
          }
      }
    }
</script>

<style scoped>

</style>
