<template>
<Home/>
<Button/>
<Getvalue/>
<CR/>
</template>
<script>
import Home from './components/Home.vue'
import Button from './components/B.vue'
import Getvalue from './components/Getvalue.vue'
import CR from './components/Cr.vue'
export default {
  name: 'App',
  components: {
    Home,
    Button,
    Getvalue,
    CR,

    }
}
</script>