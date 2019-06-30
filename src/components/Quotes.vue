<template>
  <div>

    <h5>Text you have entered</h5>
    <b-progress :value="value" :max="max" show-value class="mb-3"></b-progress>


  </div>

</template>


<script>
export default {
  name: 'Quotes',
  data () {
    return {
      value: 3,
      max: 10
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
