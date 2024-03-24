<template>
<button class="btn" v-on:click="test()">Click Me</button>
<button class="btn" v-on:click="countData()">Count Number</button>
<button class="btn" v-on:dblclick="dbclick()">Double Click</button>
<h1 style="color:white;">{{ count }}</h1>
<div class="way">
<h2>This is a 2way binding...</h2>
<input type="text" v-model="cCount"/>
<br>
<span style="font-weight: bolder;">{{ cCount }}</span>
</div>
</template>

<script>
export default{
     name:  'Button',
     data(){
          return{
               count: 0,
               cCount: '',
          }
     },
     methods:{
          test(){
               alert("ha!haaaaaaaaaa...");
          },
          dbclick(){
               alert("Haaa! Fuck me baby!");
          },
          countData(){
               this.count++;

          }
     }
}


</script>
<style scoped>
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
.way{
     color: green;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
input[type="text"]{
     padding:8px;
     width: 20%;
     background-color: rgba(128, 128, 128, 0.149);
     border: none;
     border-radius: 20px;
     color: white;
}
input[type="text"]:hover{
     cursor: text;
     background-color: rgba(128, 128, 128, 0.319);

}
</style>