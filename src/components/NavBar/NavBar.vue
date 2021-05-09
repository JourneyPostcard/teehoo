<template>
  <div class='navBarContainer'>
    <div class='navBar'>
      <img src='@/assets/logo.png' alt=''>
      <router-link to='/'>首页</router-link>
      <router-link to='/'>品牌故事</router-link>
      <router-link to='/'>在线够买</router-link>
      <router-link to='/'>联系方式</router-link>
    </div>
    <div class='navBarMobile' :class='{spread:isSpread}'>
      <div class='logoContainer'>
        <img src='@/assets/logo.png' alt='' @click='toggleSpread'>
      </div>
      <div class='linkContainer'>
        <div class='linkBg' @click='toggleSpread'></div>
        <div class='linkContent'>
          <router-link to='/'>首页</router-link>
          <router-link to='/'>品牌故事</router-link>
          <router-link to='/'>在线够买</router-link>
          <router-link to='/'>联系方式</router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import './NavBar.scss'
import './NavBar2.scss'

export default {
  data() {
    return {
      isSpread: false,
    }
  },
  methods: {
    toggleSpread() {
      this.isSpread = !this.isSpread
    },
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
