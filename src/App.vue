<template>
  <div id="app">
<Todos v-bind:todos="todos"/>    
  </div>
</template>

<script>
import Todos from './components/Todos';

export default {
  name: 'App',
  components: {
    Todos
    
  },
  data(){
    return {
      msg:'Hello',
      todos:[
        {
          id:1,
          title:"Todo One",
          compelted:false,
        },
         {
          id:2,
          title:"Todo two",
          compelted:true,
        },
         {
          id:3,
          title:"Todo three",
          compelted:false,
        },
      ]

    }
  }
}
</script>

<style>
*{
  box-sizing: border-box;
  margin:0;
  padding:0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
line-height:1.4
}
</style>
