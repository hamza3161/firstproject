<template>
  <div style="background:Black">
      <div style="color:white">
          <h1>Your Bill....</h1>
         <h4 >{{"Items Purchased "+getAll}}</h4>
         <ul >
             <li v-for="cart in products" v-bind:key="cart.id">
          <h1>{{cart.item}}</h1>
             </li>
        <!-- <li v-for="cart in getAll " v-bind:key="cart.id">
        {{getAll}}
        </li> -->
         </ul>
      </div>
  </div>
</template>

<script>
export default {
computed: {
    //   msg(){
    //     return
    // this.$store.state.cart.item;
        
    // }
    
     products(){
return this.$store.state.cart
     } ,
     getAll(){
         return this.$store.getters.getAll;
     }

  
}
,methods: {
  
},
}
</script>

<style>

</style>