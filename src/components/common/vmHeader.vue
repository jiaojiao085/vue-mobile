<template>
  <header class="vm-1px-b">
    <a class="btn-back iconfont" href="javascript:;" @click="goBack()">
      <i class="icon-back"></i>
      <span>返回</span>
    </a>
  </header>
</template>
<script>
export default {
  props: {},
  data() {
    return{
    }
  },
  methods: {
    goBack(){
      this.$router.go(-1);
    }
  }
}
</script>
<style lang="less" scoped>
header{
  z-index: 9999;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100px;
  line-height: 100px;
  background-color: white;
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  justify-content: space-between;
  a{
    &.btn-back{
      color: #333;
      padding: 0 20px;
      height: 100px;
      line-height: 100px;
      display: -webkit-box;
      display: -webkit-flex;
      display: -ms-flexbox;
      display: flex;
      i{
        font-size: 52px;
        font-style:normal;
      }
      span{
        font-size: 36px;
      }
    }
  }
}
</style>
