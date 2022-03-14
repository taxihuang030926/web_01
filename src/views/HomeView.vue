<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <p class="default">Hello Tim</p>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>

<style lang='scss' scoped>
.default{
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height:100vh;
  color:black;
  font-size: 12px;
  font-weight: 900px;
}

</style>
