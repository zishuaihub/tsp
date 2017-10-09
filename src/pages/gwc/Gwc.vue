<template>
  <div>
    <Mheader fixed titledata="GWC页面的标题"></Mheader>
    <h2>这里是GWC页面</h2>
  </div>
</template>

<script>
  import Mheader from '../../components/Mheader.vue'
  export default {
    components: {Mheader},
    name: 'GWC',
    data () {
      return {
        selected: 'gwc',
        msg: 'Welcome to Your Vue.js App'
      }
    },
  }

</script>

<style>

</style>
