<template>
  <div id="app">
   <h1>Welcome To Shopping Cart</h1>
    <!-- <todos-list/>
    <todo-form/> -->
<contact/>
<bill/>
      </div>
</template>

<script>
// import TodosList from './components/TodosList'
// import TodoForm from './components/TodoForm'

import contact from './components/Contact'
import bill from './components/Bill'

export default {
  name: 'App',
  components: {
    // TodosList,
    // TodoForm,
contact,bill
    
     
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
