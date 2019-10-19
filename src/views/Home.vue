<template>
  <div class="home">
    <el-carousel indicator-position="outside" style="display:none">
      <el-carousel-item v-for="item in 4" :key="item">
        <h3>{{ item }}</h3>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default {
  components: {}
};
</script>
<style scoped>
.home {
  width: 1200px;
  margin: 0 auto;
}
.el-carousel__item h3 {
  color: #475669;
  font-size: 18px;
  opacity: 0.75;
  line-height: 400px;
  margin: 0;
}
.el-carousel__container{
  height: 400px;
}
.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}
.el-carousel__indicators--outside{
  position: absolute;
  left: 0;
  right: 0;
}
.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
</style>