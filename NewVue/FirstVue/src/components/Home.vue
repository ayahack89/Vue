<template>
<div class="cl">
<h1>This is a home component.</h1>
<h2>Count 10 + 10 ={{ 10+10 }}</h2>
<h3>The 'string' length is {{ 'string'.length }}</h3>
<p>My name is {{ myName}}. <br> My email id {{ email }}. <br> My phone number {{ phoneNo }}. <br> I live in {{ city }}. <br> {{ getAddress() }}</p>
</div>
</template>

<script>
export  default {
     name: 'Home',
     data(){
          return{
          myName: 'Andrew',
          email : 'abcd@gmail.com',
          phoneNo: 3867594213,
          city: 'Kolkata'
          }
          
},
//Method
methods:{
     getAddress(){
          return "The  address of the person is in "+ this.city
     }
}
}
</script>

<style scoped>
.cl{
     color: green;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    
}
</style>