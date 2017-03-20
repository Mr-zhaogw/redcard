<template>
  <el-tabs v-model="activeName" @tab-click="handleClick">
    <el-tab-pane label="用户管理" name="first">1</el-tab-pane>
    <el-tab-pane label="配置管理" name="second">2</el-tab-pane>
    <el-tab-pane label="角色管理" name="third">3</el-tab-pane>
    <el-tab-pane label="定时任务补偿" name="fourth">4</el-tab-pane>
  </el-tabs>
</template>
<script>
  export default {
    data() {
      return {
        activeName: 'first'
      };
    },
    methods: {
      handleClick(tab, event) {
        console.log(tab, event);
      }
    }
  };
</script>