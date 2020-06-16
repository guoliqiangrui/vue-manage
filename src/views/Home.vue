<template>
  <div class="home">
    <!-- isHidden为true时 <img class="hidden" src="../assets/logo.png"> -->
    <img :class="{hidden: isHidden}" src="../assets/logo.png">
    <!-- <button @click="isHidden = !isHidden">{{isHidden ? '显示图片' : '隐藏图片'}}</button> -->
    <!-- @click点击事件handleShow和handleShow()带不带小括号其实没多大的区别, vue在底层会把传过去的函数统一解析成为方法, 带小括号说明有相应的实参传入方法体里面 -->
    <button @click="handleShow">{{isHidden ? '显示图片' : '隐藏图片'}}</button>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      isHidden: true
    }
  },
  methods: {
    handleShow() {
      this.isHidden = !this.isHidden;
    }
  }
}
</script>

<style scoped lang="scss">
.hidden {
  display: none;
}
</style>