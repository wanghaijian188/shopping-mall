<template>
  <div id="nav">
    <el-menu
  :default-active="activeIndex2"
  class="el-menu-demo"
  mode="horizontal"
  @select="handleSelect"
  background-color="#545c64"
  text-color="#fff"
  active-text-color="#ffd04b" style="padding:0 160px">
  <el-menu-item index="1" > <router-link to="/">Home</router-link></el-menu-item>
   <el-menu-item index="3" > <router-link to="/about">About</router-link></el-menu-item>
  <el-submenu index="2">
    <template slot="title">whj</template>
    <el-menu-item index="2-1">c</el-menu-item>
    <el-menu-item index="2-2">选项2</el-menu-item>
    <el-menu-item index="2-3">选项3</el-menu-item>
  </el-submenu>
</el-menu>
  </div>
</template>


<style>
.el-menu-vertical-demo:not(.el-menu--collapse) {
  width: 200px;
  min-height: 400px;
}
.page-component__nav{
    width: 250px;
}
.el-menu--horizontal>.el-submenu{
 float: right !important;
}
</style>

<script>
export default {
 data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
};
</script>