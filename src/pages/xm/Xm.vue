<template>
  <div>
    <Mheader fixed titledata="Xm页面的标题"></Mheader>
    <h2>这里是Xm页面</h2>
  </div>
</template>

<script>
  import Mheader from '../../components/Mheader.vue'
  export default {
    components: {Mheader},
    name: 'Xm',
    data () {
      return {
        selected: 'xm',
        msg: 'Welcome to Your Vue.js App'
      }
    },
  }

</script>

<style>

</style>
