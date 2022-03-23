<template>
  <section id ="home">
    <div id="home_section1" class="section" style="background-color: #1a1a1a">
      <img class="title_img" src="../pictures/home/home.jpeg">
    </div>
    <div id="home_section2" class="section" style="background-color: #1a1a1a">
      <div id="content1" class="content">
        <h1>こんにちは、わたしは<br><h2>Tim HUANG</h2></h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. 
          Hic, nesciunt dolorem veritatis, culpa dolores officia alias molestiae quaerat placeat 
          qui incidunt aperiam vero enim vel sint veniam ipsa? Commodi, veniam?
          </p>
      </div>
    </div>
    
  </section>  
    
</template>

<script>
// @ is an alias to /src

export default {
  name: 'HomeView',
}
</script>

<style lang='scss' scoped>
@import "@/assets/scss/home.scss";
@import "@/assets/scss/index.scss";
</style>
