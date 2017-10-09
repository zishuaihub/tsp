<template>
  <div>
    <Mheader fixed titledata="MDT页面的标题"></Mheader>
<h2>这里是MDT页面</h2>
  </div>
</template>

<script>
  import Mheader from '../../components/Mheader.vue'
  export default {
    components: {Mheader},
    name: 'HelloWorld',
    data () {
      return {
        selected: 'mdt',
        msg: 'Welcome to Your Vue.js App'
      }
    },
  }

</script>

<style>

</style>
