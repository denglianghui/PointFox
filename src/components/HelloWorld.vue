<template>
  <div class="hello">
     <el-container id="wrapper">
            <el-header id="indexHeader">
                <div id="headerTitle">
                    江西软件大学-新型图书管理系统
                </div>
                <div id="headerFunction">
                    <el-button type="primary" disabled>系统登录</el-button>
                    <el-button type="primary" disabled>工作中心</el-button>
                    <el-button type="primary" disabled>学生信息查询</el-button>
                    <el-button type="primary" disabled>图书信息查询</el-button>
                </div>
            </el-header>
            <el-main id="indexMain">
                <el-card class="box-card" id="loginCard">
                    <div slot="header" class="clearfix">
                      <span>系统登录</span>
                      <el-button style="float: right; padding: 3px 0" type="text">找回密码</el-button>
                    </div>
                    <div id="loginContent">
                        <el-input clearable v-model="user.username"></el-input>
                        <el-input clearable v-model="user.password" show-password></el-input>
                        <el-button id="loginSystem">登录</el-button>
                    </div>
                  </el-card>
            </el-main>
            <el-footer id="indexFooter">
                <div id="footerContent">
                    <div id="tip1">
                        通信地址：江西省南昌市湾里区江西软件大学 邮编：330041
                    </div>
                    <div id="tip2">
                        &copy; 版权属于江西软件大学 2020-2021
                    </div>
                </div>
            </el-footer>
          </el-container>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      user: {
        username: "",
        password: "",
      },
    };
  },

  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
