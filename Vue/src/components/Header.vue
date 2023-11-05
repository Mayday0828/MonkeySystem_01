<template>
  <div style="display: flex;line-height: 50px; justify-content: space-between">
    <div>
      <i class="el-icon-s-fold" style="font-size: 20px; line-height: 50px;"></i>
    </div>
    <div>
    <span>郑嘉豪</span>
    <el-dropdown>
      <i class="el-icon-arrow-down"  style="margin-left: 1px"></i>
      <el-dropdown-menu slot="dropdown">
         <el-dropdown-item @click.native="toUser">个人中心</el-dropdown-item>
         <el-dropdown-item @click.native="logout">用户管理</el-dropdown-item>
         <el-dropdown-item @click.native="">消息</el-dropdown-item>
         <el-dropdown-item @click.native="logout">退出登录</el-dropdown-item>
      </el-dropdown-menu>
    </el-dropdown>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  methods:{
    toUser(){
      console.log('to_user')
    },
    logout(){
      console.log('logout')
    }
  }
}
</script>

<style scoped>

</style>
