<template>
  <div id="app">

    <Quotes/>
    <input/>
    <router-view/>
  </div>
</template>

<script>

  import Quotes from "./components/Quotes";
  import input from "./components/input"
  export default {
    name: 'App',
    components: Quotes,
     input
  }
</script>

<style>

</style>
