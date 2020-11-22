<template>
<div>
  <Login/>
<router-view></router-view>
</div>
</template>

<script>
import Login from './components/Login.vue'
//import Browse from './components/Browse.vue'
//import Index from './components/Index.vue'

export default {
  name: 'App',
  components: {
    Login
    
  }
}
</script>

<style scoped src="./components/style.css">
</style>
