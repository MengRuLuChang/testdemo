<template>
  <div id="app">
   <shoppingcart></shoppingcart>
   <shopping-search></shopping-search>
  </div>
</template>

<script>
import shoppingcart from "./components/shopping-cart";
import shoppingSearch from "./components/shopping-search";
export default {
  name: 'app',
  data () {
    return {
      
    }
  },
  components:{
    shoppingcart,
    shoppingSearch
  }
}
</script>

<style>
</style>
