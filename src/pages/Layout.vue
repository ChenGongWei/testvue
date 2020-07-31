<template>
  <div>
    <el-container>
      <!-- 侧边导航栏 -->
      <el-aside width="200px">
        <Aside></Aside>
      </el-aside>
      <!-- 主体 -->
      <el-container>
        <!-- 头部 -->
        <el-header>
          <span>admin</span>
          <i class="el-icon-setting"></i>
        </el-header>
        <!-- 内容 -->
        <el-main>
          <!-- 面包屑导航 -->
          <el-breadcrumb separator="/">
            <el-breadcrumb-item :to="{ path: '/' }">首页</el-breadcrumb-item>
            <el-breadcrumb-item>菜单列表</el-breadcrumb-item>
          </el-breadcrumb>
          <!-- 展示内容 -->
          <Main />
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import Aside from "./Aside";
import Main from "./Main";

export default {
  components: {
    Aside,
    Main,
  },
};
</script>

<style scoped>
.el-header {
  background-color: #b3c0d1;
  color: #333;
  text-align: right;
  line-height: 60px;
}

.el-aside {
  background-color: #d3dce6;
  color: #333;
  text-align: center;
  /* line-height: 200px; */
}

.el-main {
  background-color: #e9eef3;
  color: #333;
  height: 440px;
  overflow-y: auto;
  /* text-align: center; */
  /* line-height: 160px; */
}

/* body > .el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
} */
</style>