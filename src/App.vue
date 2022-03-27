<template>
  <div class="app">
    <Header></Header>
    <router-view/>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "./components/header.vue"
import Footer from "./components/footer.vue"
export default {
  name:'App',
  components:{
    Header,
    Footer 
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Josefin+Sans:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;1,100;1,200;1,300;1,400;1,500;1,600;1,700&display=swap');

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family:'Josefin Sans', Arial, Helvetica, sans-serif;
    scroll-behavior: smooth;
}

.deafult{
    position:relative;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    color: #000;
    font-size: 18vw;
    font-weight: 700;
}
</style>

<style lang="scss">
@import "@/assets/scss/index.scss";
</style>
