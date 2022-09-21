<template>
  <el-container class="container">
    <el-aside width="200px" class="aside">
      <p class="text">Aside</p>
    </el-aside>
    <el-container>
      <el-header class="header">
        <p>Header</p>
      </el-header>
      <el-main class="main">
        <p>Main</p>
        <el-button @click="open">默认按钮</el-button>
        <el-button type="primary">主要按钮</el-button>
        <el-button type="success">成功按钮</el-button>
        <el-button type="info">信息按钮</el-button>
        <el-button type="warning">警告按钮</el-button>
        <el-button type="danger">危险按钮</el-button>
      </el-main>
      <el-footer height="20px" class="footer"></el-footer>
    </el-container>
  </el-container>
</template>

<script>
export default {
  methods: {
    open() {
      this.$message('这是一条消息提示');
    },
  },
};
</script>

<style lang="less" scoped>
.container {
  height: 100%;
}
.aside {
  background-color: rgb(29, 123, 174);
}
.header {
  background-color: rgba(29, 123, 174, 0.228);
}
.main {
  height: 100%;
  background-color: white;
}
.footer {
  background-color: rgb(239, 239, 239);
}
.text {
  color: rgb(255, 255, 255);
}
</style>
