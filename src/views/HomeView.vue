<template>
  <div class="home">
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/header.vue'

export default {
  name: 'HomeView',
  components: {
    Header
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
