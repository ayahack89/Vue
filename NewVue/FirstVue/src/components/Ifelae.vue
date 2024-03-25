<template>
<div class="ifelse">
<h2>If else statement</h2>
<span v-if="show">Show: ON</span>
<span v-else>Show: OFF</span>
<button type="button" v-on:click="show=!show" class="btn">Toggel</button>
</div>
</template>

<script>
export default{
     name : 'Ifelse',
     data(){
          return{
               show:true,
               
          }
     }
}
</script>

<style>
.ifelse{
     color: green;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
.btn{
     width: 10%;
     margin: 20px;
     padding: 8px;
     font-size: 1rem;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
     background-color: green;
     color: rgb(153, 255, 0);
     border-radius: 50px;
     border: none;
}
.btn:hover{
     cursor: pointer;
     transform: scale(1.1);
}
</style>