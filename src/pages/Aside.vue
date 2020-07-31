<template>
  <div>
    <el-menu
      default-active="2-1"
      class="el-menu-vertical-demo"
      @open="handleOpen"
      @close="handleClose"
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b"
    >
      <h3>后台管理系统</h3>

      <!-- 首页 -->
      <el-menu-item index="1">
        <i class="el-icon-s-home"></i>
        <span slot="title">首页</span>
      </el-menu-item>

      <!-- 系统设置 -->
      <el-submenu index="2">
        <template slot="title">
          <i class="el-icon-setting"></i>
          <span slot="title">系统设置</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="2-1">菜单管理</el-menu-item>
          <el-menu-item index="2-2">角色管理</el-menu-item>
          <el-menu-item index="2-3">管理员管理</el-menu-item>
        </el-menu-item-group>
      </el-submenu>

      <!-- 产品管理 -->
      <el-submenu index="3">
        <template slot="title">
          <i class="el-icon-s-goods"></i>
          <span slot="title">产品管理</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="3-1">菜单管理</el-menu-item>
          <el-menu-item index="3-2">角色管理</el-menu-item>
          <el-menu-item index="3-3">管理员管理</el-menu-item>
        </el-menu-item-group>
      </el-submenu>

      <!-- 商城管理 -->
      <el-submenu index="4">
        <template slot="title">
          <i class="el-icon-user-solid"></i>
          <span slot="title">商城管理</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="4-1">菜单管理</el-menu-item>
          <el-menu-item index="4-2">角色管理</el-menu-item>
          <el-menu-item index="4-3">管理员管理</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
    </el-menu>
  </div>
</template>

<script>
export default {
  methods: {
    handleOpen(key, keyPath) {
      console.log(key, keyPath);
    },
    handleClose(key, keyPath) {
      console.log(key, keyPath);
    },
  },
};
</script>

<style>
h3 {
  color: #eee;
  font-weight: normal;
  margin: 10px 20px;
}
.el-menu-vertical-demo {
  height: 500px;
  text-align: left;
}
.el-submenu .el-menu-item {
  min-width: 180px;
}
</style>