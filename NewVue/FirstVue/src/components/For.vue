<template>
<div class="for">
<h2>For loop in Vue.</h2>
<h3>My friends..</h3>
<ul>
<li v-for="friends in myfriends" :key="friends">{{ friends }}</li>
</ul>
<br>
<br>
<h3>My friends name with email.</h3>

     <span v-for="item in n_emal" :key="item.email">
          <ul>
           <li>Name: {{ item.name }}</li>  
          <li>Email: {{ item.email }}</li>
          </ul>
     </span>
</div>
</template>

<script>
export default{
     name: 'For', 
     data(){
          return {
               myfriends: ['Agnik', 'Swrup', 'Shivam', 'Jeet', 'Vivak'],
               n_emal: [
                    {
                         name: 'Agnik',
                         email: 'agnik@gmail.com'
                    },
                    {
                         name: 'Swrup',
                         email: 'swrup@yahoo.com'
                    },
                    {
                         name: 'Shivam',
                         email: 'shivam@hotmail.com'
                    },
                    {
                         name: 'Jeet',
                         email: 'jeet1234567890@outlook.com'
                    },
                    {
                         name: 'Vivak',
                         email: 'vivakjethva@rediffmail.com'
                    },
               ]
          }
     }
}
</script>

<style>
.for{
     color: green;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
ul, li{
     list-style-type: none;
}
</style>