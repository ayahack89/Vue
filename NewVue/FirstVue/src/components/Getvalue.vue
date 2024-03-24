<template>
<div class="get">
     <h2>Get value by inputs.</h2>
     <input type="email" v-model="email"/><br><br><input type="number" v-model="phone"/>
     <br>
     <button class="btn" type="button" v-on:click="getData()">Get Value</button>
     <br>
     <span>Email: {{email}}</span><br><span>Phone: {{ phone }}</span>
</div>
</template>

<script>
export default{
     name: 'Getvalue',
     data(){
          return {
               email: null,
               phone: null

          }
     }
     ,
     methods:{
          getData(){
               console.log("Hellow!", this.email, this.phone);
          }

     }
}
</script>
<style>
.get{
     color: green;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
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
input[type="email"],
input[type="number"]
{
     padding:8px;
     width: 20%;
     background-color: rgba(128, 128, 128, 0.149);
     border: none;
     border-radius: 20px;
     color: white;
}
input[type="email"]:hover{
     cursor: text;
     background-color: rgba(128, 128, 128, 0.319);

}
input[type="number"]:hover{
     cursor: text;
     background-color: rgba(128, 128, 128, 0.319);

}

</style>