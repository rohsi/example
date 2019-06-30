<template>
  <div id="app">

<Quotes/>
    <router-view/>
  </div>
</template>

<script>

import Quotes from "./components/Quotes";
export default {
  name: 'App',
  components: Quotes
}
</script>

<style>

</style>
