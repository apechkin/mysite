<template lang="html">
  <div class="header">
    <ul v-for="(element, index) in header"  :key="index">
      <li>{{element.toUpperCase()}}</li>
    </ul>
  </div>
</template>

<script>
import _ from 'lodash'
export default {
  name: 'Header',
  data () {
    return {
      header: [ 'home', 'about', 'experience', 'education', 'skills', 'contact' ]
    }
  }
}
</script>

<style lang="less">
.header {
  display: flex;
  width: 1176px;
  margin-left: auto;
  margin-right: auto;
  justify-content: space-around;
}
</style>
