<template>
  <div id="headerBook">
    <el-header id="indexHeader">
      <div id="message">{{ message }}</div>
      <div id="headerFunction">
        <router-link to="login">
        <el-button type="primary" disabled>系统登录</el-button>
        </router-link>
        <router-link to="work">
        <el-button type="success" disabled>工作中心</el-button>
        </router-link>
        <router-link to="/student">
        <el-button type="warning" disabled>学生信息查询</el-button>
        </router-link>
        <router-link to="/book">
        <el-button type="danger" disabled>图书信息查询</el-button>
        </router-link>
        <router-link to="/cnnode">
        <el-button>node论坛</el-button>
        </router-link>
      </div>
    </el-header>
  </div>
</template>

<script>
export default {
  name: "headerBook",
  data() {
    return {
      message: "江西软件大学-新型图书管理系统",
    };
  },
};
</script>

<style scoped>
#headerBook {
  background-color: #244152;
}
#message {
  width: 500px;
  /*  background-color: red; */
  color: #0a9588;
  font-size: 30px;
  font-weight: bolder;
  height: 60px;
  line-height: 60px;
  display: inline-block;
}
#headerFunction {
  /* float: right; */
  display: inline-block;
  /* width: 200px; */
  height: 60px;
  /* background-color:green; */
}
#headerFunction > .el-button {
  display: inline-block;
  margin-top: 8px;
  background-color: #0a9588;
}
</style>