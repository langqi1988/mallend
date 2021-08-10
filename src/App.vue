<template>
  <div id="app">
    <router-view></router-view>
    <tab-bar>
      <template #default>
        <tab-bar-item
          path='/home'
          
        >
          <template v-slot:item-icon>
            <img
              src="./assets/img/tabbar/home.svg"
              alt=""
            >
          </template>
          <template v-slot:item-icon-active>
            <img
              src="./assets/img/tabbar/home_active.svg"
              alt=""
            >
          </template>
          <template #item-text>
            <div>首页</div>
          </template>
        </tab-bar-item>
        <tab-bar-item path='/category'>
          <template v-slot:item-icon>
            <img
              src="./assets/img/tabbar/category.svg"
              alt=""
            >
          </template>
          <template v-slot:item-icon-active>
            <img
              src="./assets/img/tabbar/category_active.svg"
              alt=""
            >
          </template>
          <template #item-text>
            <div>分类</div>
          </template>
        </tab-bar-item>
        <tab-bar-item path='/cart'>
          <template v-slot:item-icon>
            <img
              src="./assets/img/tabbar/shopcart.svg"
              alt=""
            >
          </template>
          <template v-slot:item-icon-active>
            <img
              src="./assets/img/tabbar/shopcart_active.svg"
              alt=""
            >
          </template>
          <template #item-text>
            <div>购物车</div>
          </template>
        </tab-bar-item>
        <tab-bar-item path='/profile'>
          <template v-slot:item-icon>
            <img
              src="./assets/img/tabbar/profile.svg"
              alt=""
            >
          </template>
          <template v-slot:item-icon-active>
            <img
              src="./assets/img/tabbar/profile_active.svg"
              alt=""
            >
          </template>
          <template #item-text>
            <div>我的</div>
          </template>
        </tab-bar-item>
      </template>
    </tab-bar>
  </div>
</template>

<script>
import TabBar from "./components/tabbar/TabBar.vue";
import TabBarItem from "./components/tabbar/TabBarItem.vue";
export default {
  name: "App",
  components: {
    TabBar,
    TabBarItem,
  },
};
</script>

<style>
@import url("./assets/css/base.css");
</style>
