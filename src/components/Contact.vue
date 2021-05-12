<template>
  <div class="container" style="background:Green">
<div class="row" style="color:white"> 
          
          <h3 >Iphone 11, Price:120000</h3>
          <button @click="addToCart('Iphone 11,Price:120000')">Add to Cart</button>
            
          <h3 >Samsung S10, Price:201000</h3>
          <button  @click="addToCart('Samsung S10 , Price:201000')">Add to Cart</button>
 </div>
 <div> 
     
 </div>
  </div>
</template>

<script>
export default {

methods: {
    
    addToCart(item){
    // alert("Add ho gaya");
    this.$store.dispatch("addtoCart",item);
    console.log("add ho ga",item);
    }
},
}
</script>

<style>

</style>