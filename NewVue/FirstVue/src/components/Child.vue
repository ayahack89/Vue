<template>
<div class="child">
     <h5>This is a child component.</h5>
     <span>Child: {{ name }} </span>
     <span><br> Name: {{ user.name }} <br> Email: {{ user.email }} <br> Age: {{ user.age }} <br> Country: {{ user.country }}</span>
</div>
</template>

<script>
export default{
     name: 'Child',
    props:{
     name:String,
     user:Object,


    }
}
</script>

<style>
.child{
     color:green ;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

</style>