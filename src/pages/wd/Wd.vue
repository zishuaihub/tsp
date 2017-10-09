<template>
  <div>
    <Mheader fixed titledata="Wd页面的标题"></Mheader>
    <h2>这里是Wd页面</h2>
  </div>
</template>

<script>
  import Mheader from '../../components/Mheader.vue'
  export default {
    components: {Mheader},
    name: 'Wd',
    data () {
      return {
        selected: 'wd',
        msg: 'Welcome to Your Vue.js App'
      }
    },
  }

</script>

<style>

</style>
