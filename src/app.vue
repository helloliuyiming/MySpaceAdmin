<template>
  <el-container>
    <el-header>Header</el-header>
    <el-container>
      <el-aside>

        <el-menu default-active="1-4-1" class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose" :collapse="isCollapse">
          <el-sub-menu index="1">
            <template #title>
              <i class="el-icon-location"></i>
              <span>首页</span>
            </template>
          </el-sub-menu>
          <el-sub-menu index="2">

            <template #title>
              <i class="el-icon-menu"></i>
              <span>权限管理</span>
            </template>
          </el-sub-menu>
          <el-sub-menu index="3">

            <template #title><i class="el-icon-document"></i><span>订阅管理</span></template>
          </el-sub-menu>
          <el-sub-menu index="4">

            <template #title><i class="el-icon-setting"></i><span>数据管理</span></template>
            <el-menu-item>Blog</el-menu-item>
            <el-menu-item>TODO</el-menu-item>
            <el-menu-item>Moment</el-menu-item>
          </el-sub-menu>
          <el-sub-menu index="5">

            <template #title><i class="el-icon-setting"></i><span>系统设置</span></template>
          </el-sub-menu>
        </el-menu>
      </el-aside>
      <el-container>
        <el-main>Main</el-main>
        <el-footer>MySpace-Admin power by Lym</el-footer>
      </el-container>
    </el-container>
  </el-container>
</template>

<script>
export default {
  name: "app"
}
</script>

<style scoped>
.el-header, .el-footer {
  background-color: #B3C0D1;
  color: var(--el-text-color-primary);
  text-align: center;
  line-height: 60px;
}

.el-aside {
  background-color: #D3DCE6;
  color: var(--el-text-color-primary);
  text-align: center;

}

.el-main {
  background-color: #E9EEF3;
  color: var(--el-text-color-primary);
  text-align: center;
  line-height: 160px;
}

body > .el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>
