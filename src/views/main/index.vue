<template>
  <el-container>
    <el-aside width="200px">
      <div class="title-wrapper">
        <img src="../../assets/cow.jpg" alt="">
        <span id="span">xx后台管理系统</span>
      </div>

      <el-scrollbar class="scrollerbar">
        <el-menu
            default-active="1"
            class="el-menu-vertical-demo"
        >

          <el-menu-item index="1">
            <i class="el-icon-menu"></i>
            <span slot="title">首页</span>
          </el-menu-item>
          <el-submenu index="2">
            <template slot="title">
              <i class="el-icon-location"></i>
              <span>商品管理</span>
            </template>
            <el-menu-item index="2-1">
              <i class="el-icon-menu"></i>
              <span slot="title">品牌管理</span>
            </el-menu-item>
            <el-menu-item index="2-2">
              <i class="el-icon-menu"></i>
              <span slot="title">分类管理</span>
            </el-menu-item>
            <el-menu-item index="2-3">
              <i class="el-icon-menu"></i>
              <span slot="title">商品管理</span>
            </el-menu-item>
          </el-submenu>

          <el-menu-item index="3">
            <i class="el-icon-menu"></i>
            <span slot="title">运营商管理</span>
          </el-menu-item>

        </el-menu>
      </el-scrollbar>


    </el-aside>

    <el-container>
      <el-header>Header</el-header>
      <el-main>Main</el-main>
    </el-container>
  </el-container>
</template>

<script>
export default {
  name: "index"
}
</script>

<style scoped lang="less">
.el-header {
  background-color: #f56c6c;
  color: #fff;
  text-align: center;
  line-height: 60px;
}

.scrollerbar {
  height: 867px;
}

.el-aside {
  background-color: #fff;
  color: #444;

  .title-wrapper {
    line-height: 60px;
    background-color: #f56c6c;
  }

  img {
    width: 35px;
    height: 35px;
    border-radius: 50%;
    vertical-align: middle;
    margin: 0 8px 0 10px;
  }

  #span {
    font-weight: 700;
    color: #ffffff;
    font-size: 18px;
  }
}

.el-main {
  background-color: #E9EEF3;
  color: #444;
  text-align: center;
}

.el-container {
  margin-bottom: 40px;
  width: 100%;
  height: 100%;
}



</style>