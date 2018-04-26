<template lang="html">
  <div class="header">
    <div class="logo">
      This is logo
    </div>
    <div class="menu">
      <ul v-for="(element, index) in header"  :key="index">
        <li><a href="#" class="menu-link" />{{element.toUpperCase()}}</li>
      </ul>
    </div>
  </div>
</template>

<script>
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
  justify-content: space-between;
  width: 60%;
  height: 20vh;
  border: 2px solid red;
  align-items: center;
}
.menu {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  width: 60%;
  ul {
    list-style: none;
    color: #00796B;
    li:hover {
      color: #E0F2F1
    }
  }
}

</style>
