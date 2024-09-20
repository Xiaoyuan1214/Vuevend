<template>
  <div>
    <button v-on:click="addFunds(1)">$1</button>
    <button v-on:click="addFunds(5)">$5</button>
    <button v-on:click="addFunds(10)">$10</button>
  </div>
</template>

<script>
export default {
  methods: {
    addFunds(amount){
      this.$store.commit("INCREASE_FUNDS", amount);
    }
  }

}
</script>

<style>
  button{
    width:150px;
    margin:10px;
    border-radius: 20px;

  }
</style>