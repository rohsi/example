<template>
  <div id="app">

<Quote/>
    <router-view/>
  </div>
</template>

<script>


  import Quote from "./components/Quote";
  export default {
    name: 'App',
    components: {Quote},
    data() {
      return {

      }
    },
    methods: {
      enter() {
        this.message=[]
      }
    },
  }
</script>

<style>

</style>
