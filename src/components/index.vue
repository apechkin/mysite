<template>
  <div id="app">
    <div class="conteiner">
      <div class="content">
        <header-layout />
        <router-view/>
      </div>
    </div>
    <div class="side">
      Side
    </div>
    <div class="footer">
      Footer
    </div>
  </div>
</template>

<script>
import HeaderLayout from './Layout/header.vue'
export default {
  name: 'App',
  components: {
    HeaderLayout
  }
}
</script>

<style lang="less">
@import './assets/global.less';
</style>
