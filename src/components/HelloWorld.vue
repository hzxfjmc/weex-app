<template>
    <div class="navlist">
      <div class="nav" v-for="(item,index) in navList" :key="index">
        <text class="name">{{item.name}}</text>
      </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
      navList: [
        { name: "首页" },
        { name: "订单" },
        { name: "购物车" },
        { name: "我的" }
      ]
    };
  },
  methods: {
    handlerImages() {
      console.log(123);
    }
  }
};
</script>

<style scoped>
.navlist {
  width: 750px;
  height: 100px;
  display: flex;
  flex-direction: column;
  position:fixed;
  border-width:1px;
  bottom:0;
  border-color:red;
}
.nav {
  flex-grow:1;
  text-align: center;
}
.nav .name{
  width:100%;
  text-align: center;
}
</style>