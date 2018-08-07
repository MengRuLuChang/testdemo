<template>
  <div id="app">
   <shoppingcart></shoppingcart>
  </div>
</template>

<script>
import shoppingcart from "./components/shopping-cart"
export default {
  name: 'app',
  data () {
    return {
      
    }
  },
  components:{
    shoppingcart
  }
}
</script>

<style>
</style>
