<template>
    <div>
      <input type="text" v-model="message">

      <button v-on:click="enter">ENTER</button>
      <p> {{feedback}}</p>
      <p>{{message}}</p>
      <div v-for="(quote,index) in quotes" :key="index">

        <p v-on:click="deletearray(index)">{{quote}}</p>
      </div>
    </div>
</template>

<script>
    export default {
        name: "Quote",
      data() {
        return{
          message:'',
          feedback:null,
          quotes:[]
        }
      },
      methods: {
        enter() {
          if (this.quotes.length<10){
            this.quotes.push(this.message)

          } else {
            this.message=null;
            this.feedback='delete text' ;
          }
        }
      },
      deletearray:function(index){
       this.quotes.splice( index, 1 );
      }


    }
</script>

<style scoped>

</style>
