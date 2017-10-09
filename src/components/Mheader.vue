<template>
  <div>
      <mt-header fixed :title="titledata">
        <router-link to="/" slot="left">
          <mt-button icon="back" @click.Native="test()">返回</mt-button>
        </router-link>
        <mt-button >关闭</mt-button>
        <mt-button icon="more" slot="right"></mt-button>
      </mt-header>

  </div>
</template>

<script>
    export default {
      name: 'header',
      props: ['titledata'],
      data(){
        return{
        }
      },
      methods: {
        test: function () {
          alert(this.titledata)
        }
      }
    }
</script>

<style>

</style>
