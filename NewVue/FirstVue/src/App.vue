<template>
<Home/>
<Button/>
<Getvalue/>
<CR/>
<Ifelse/>
<For/>
<Parent/>
</template>
<script>
import Home from './components/Home.vue'
import Button from './components/B.vue'
import Getvalue from './components/Getvalue.vue'
import CR from './components/Cr.vue'
import Ifelse from './components/Ifelae.vue'
import For from './components/For.vue'
import Parent from './components/Parent.vue'
export default {
  name: 'App',
  components: {
    Home,
    Button,
    Getvalue,
    CR,
    Ifelse,
    For,
    Parent,

    }
}
</script>