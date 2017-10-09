<template>

  <div class="hello">

    <mt-tab-container v-model="selected">
      <mt-tab-container-item id="mdt">
        <!--<mt-cell v-for="n in 10" title="tab-container 1"></mt-cell>-->
        <template>
          <div class="page-swipe">
            <mt-swipe :auto="0">
              <mt-swipe-item class="slide1">1</mt-swipe-item>
              <mt-swipe-item class="slide2">2</mt-swipe-item>
              <mt-swipe-item class="slide3">3</mt-swipe-item>
            </mt-swipe>
          </div>
          <div class="page-swipe">
            <mt-swipe :auto="0" :continuous="false">
              <mt-swipe-item class="slide1">1</mt-swipe-item>
              <mt-swipe-item class="slide2">2</mt-swipe-item>
            </mt-swipe>
          </div>
        </template>
        <Mdt></Mdt>
      </mt-tab-container-item>
      <mt-tab-container-item id="xm">
        <mt-cell v-for="n in 5" title="tab-container 2"></mt-cell>
        <Xm></Xm>
      </mt-tab-container-item>
      <mt-tab-container-item id="gwc">
        <Gwc></Gwc>
        <mt-cell v-for="n in 7" title="tab-container 3"></mt-cell>
      </mt-tab-container-item>
      <mt-tab-container-item id="wd">
        <mt-cell v-for="n in 7" title="tab-container 4"></mt-cell>
        <Wd></Wd>
      </mt-tab-container-item>
    </mt-tab-container>

    <mt-tabbar fixed v-model="selected">
      <mt-tab-item id="mdt">
        <img slot="icon" src="../assets/logo.png" alt="">
        免单团
      </mt-tab-item>
      <mt-tab-item id="xm">
        <img slot="icon" src="../assets/logo.png" alt="">
        寻觅
      </mt-tab-item>
      <mt-tab-item id="gwc">
        <img slot="icon" src="../assets/logo.png" alt="">
        购物车
      </mt-tab-item>
      <mt-tab-item id="wd">
        <img slot="icon" src="../assets/logo.png" alt="">
        我的
      </mt-tab-item>
    </mt-tabbar>
  </div>
</template>

<script>
  import Mdt from '../pages/mdt/Mdt.vue'
  import Xm from '../pages/Xm/Xm.vue'
  import Gwc from '../pages/Gwc/Gwc.vue'
  import Wd from '../pages/Wd/Wd.vue'
  export default {
    components: {Mdt, Xm, Gwc, Wd},
    name: 'HelloWorld',
    data () {
      return {
        selected: 'mdt',
        msg: 'Welcome to Your Vue.js App'
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scped>
    .page-swipe-desc {
    text-align: center;
    color: #666;
    margin-bottom: 5px;
  }
    .mint-swipe {
      height: 200px;
      color: #fff;
      font-size: 30px;
      text-align: center;
      margin-bottom: 20px;
    }
    .mint-swipe-item {
      line-height: 200px;
    }
    .slide1 {
      background-color: #0089dc;
      color: #fff;
    }
    .slide2 {
      background-color: #ffd705;
      color: #000;
    }
    .slide3 {
      background-color: #ff2d4b;
      color: #fff;
    }
</style>
