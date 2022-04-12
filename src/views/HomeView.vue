<template>
  <section id ="home">

    <div id="home_section1" class="section" style="background-color: #1a1a1a">
      <img class="title_img" src="../pictures/home/home.png">
    </div>

    <div id="home_section2" class="section" style="background-color: #1a1a1a">
      <div id="content1" class="content">
        <h1>こんにちは<br><h2>Tim HUANG</h2></h1>
        <p style="color: white"> 
          Here will be some brief introduction to myself.
        </p>
      </div>
    </div>

    <div id="home_section3" class="section" style="background-color: #1a1a1a">
      <div id="content2" class="content">
        <h1>Gallery</h1>
        <p style="color: white">
          [Under Contruction!]
          Here will be a gallery of photos I took and videos I made
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
