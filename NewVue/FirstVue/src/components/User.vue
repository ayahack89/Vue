<template>
<div class="user">
     <h2>Reuse component</h2>
     <div>
          <ul>
               <li>{{ u.name }}</li>
               <li>{{ u.email }}</li>
               <li>{{ u.age }}</li>
               <li>{{ u.country }}</li>
          </ul>
     </div>
</div>
</template>

<script>
export default{
     name: 'User',
     props:{
          item:Object,
     }
}
</script>

<style>
.user{
     border: 2px solid green;
     width: 20%;
     margin: auto;
     color: green;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
</style>