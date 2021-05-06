<template>
  <div id='app' class='nonConvertWhenPC'>
    <NavBar/>
    <router-view/>
    <BottomBar/>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar/NavBar.vue'
import BottomBar from '@/components/BottomBar/BottomBar.vue'

export default {
  components: {
    NavBar,
    BottomBar,
  },
}
</script>

<style>
body {
  margin:0;
  padding:0;
  border:0;
  font-size:12px;
  font-family:PingFangSC-Semibold sans-serif;
  background-color:#f8f8f8;
  color:#666;
  -webkit-text-size-adjust:none;
  /*user-select:none;*/
}
img, a, p, span, h1, h2, h3, ul, ol, li, select, input, dl, dt, dd, table, tr, td, em, div {
  padding:0;
  margin:0;
  border:0;
  text-decoration:none;
  list-style:none;
  font-style:normal;
  -webkit-tap-highlight-color:rgba(255, 255, 255, 0);
}
select, input, img {
  vertical-align:middle;
  -webkit-appearance:none;
  outline:none;
}

</style>
