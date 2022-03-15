<template>
  <header :class="{ 'scrolled-nav': scrollNav}">
        <nav>
            <router-link to="/" class="logo">Tim Huang</router-link>
            <ul v-show="!mobile" class="navigation">
                <li><router-link to="/">Home</router-link> </li>
                <li><router-link to="/about">About</router-link> </li>
                <li><router-link to="/project">Project</router-link> </li>
                <li><router-link to="/news">News</router-link> </li>
                <li><router-link to="/blog">Blog</router-link> </li>
                <li><router-link to="/contact">Contact</router-link> </li>
           </ul>
            <div class="navbar_icon">
                <i @click="toggleMobileNav" v-show="mobile" class="fi fi-br-menu-burger" :class="{'icon-active':mobileNav}" ></i>
            </div>
            <transition name='mobile-nav'>
                <ul v-show="mobileNav" class="dropdown-nav">
                  <li><router-link to="/">Home</router-link> </li>
                  <li><router-link to="/about">About</router-link> </li>
                  <li><router-link to="/project">Project</router-link> </li>
                  <li><router-link to="/news">News</router-link> </li>
                  <li><router-link to="/blog">Blog</router-link> </li>
                  <li><router-link to="/contact">Contact</router-link> </li>
                </ul>
            </transition>
        </nav>
      </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return{
          scrollNav: null,
          mobile: null,
          mobileNav: null,
          windowWidth: null,
      };
    },
    created(){
        window.addEventListener('resize', this.checkScreen);
        this.checkScreen();
    },
    mounted(){
        window.addEventListener('scroll', this.updateSroll);
    },
    methods:{
        toggleMobileNav(){
            this.mobileNav = !this.mobileNav;
        },

        updateSroll(){
            const scrollPosition = window.scrollY;
            if(scrollPosition > 50){
                this.scrollNav = true;
                return;
            }
            this.scrollNav = false;
        },
        checkScreen(){
            this.windowWidth = window.innerWidth;
            if(this.windowWidth <= 850){
                this.mobile = true;
                return
            }
            this.mobile = false;
            this.mobileNav = false;
            return;
        },
    },
};
</script>

<style lang="scss" scoped>
  @import "../assets/scss/header.scss"
</style>