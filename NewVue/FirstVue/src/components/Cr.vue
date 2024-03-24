<template>
<div class="cr">
<h3>Check Box and Radio Button</h3>
<label for="Java">Java</label>
<input type="checkbox" id="Java" value="Java" v-model="technology">
<br>
<label for="Php">Php</label>
<input type="checkbox" id="Php" value="PHP" v-model="technology">
<br>
<label for="NodeJs">NodeJs</label>
<input type="checkbox" id="NodeJs" value="NodeJs" v-model="technology">
<br>
<span>Technology: {{technology}}</span>
<br>
<label for="who">Student</label>
<input type="radio" id="radio" value="Student" v-model="who" />
<label for="who">Developer</label>
<input type="radio" id="radio" value="Developer" v-model="who" />
<br>
<span>I am..{{who}}</span>
</div>
</template>

<script>
export default{
     name: 'CR',
     data(){
          return {
               technology: [],
               who:null,
          }
     }

}
</script>

<style>
.cr{
     color:Green;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;

}
</style>