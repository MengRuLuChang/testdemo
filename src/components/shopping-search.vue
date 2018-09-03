<template>
    <div class="sorting">
        <label for="filtername">Find your hero:</label>
        <input type="text" v-model="findName" id="filtername"/>
        <ul>
            <li v-for="name in filteredNmaes">{{ name }}</li>
        </ul>
    </div>
</template>
<script>
export default {
   data(){
       return {
           findName: '',
           names:[
               "aa",
               "aac",
               "ab",
               "av",
               "ac",
               "ss",
               "vvf",
               "bbd",
               "ccf",
               "ggd",
               "sda",
           ]
       }
   },
   computed:{
       filteredNmaes:function(){
           let filter =  new RegExp( this.findName, 'i' );
           return this.names.filter( el => el.match(filter))
       }
   }
 
};
</script>

