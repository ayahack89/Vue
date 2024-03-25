<template>
<div class="parent">
     <h2>This is a parent component.</h2>
     <!-- <span>Name: {{ name }}</span> -->
     <Child name="Andrew" :user="user"/>
</div>
</template>

<script>
import Child from './Child.vue'
export default{
     name: 'Parent',
     components: {
          Child
     },
     data(){
          return{
               user: 
               {
                    name: "John Doe", 
                    email: "john@doe.com", 
                    age: 30, 
                    country: "USA",
               }
          }
     }
}
</script>

<style>
.parent{
     color: green;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
</style>