<template>
  <div id="nav">
 
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