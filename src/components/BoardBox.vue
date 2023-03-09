<template>
  <div class="board_box">
    <div class="header_img">
      <el-avatar src="https://cube.elemecdn.com/0/88/03b0d39583f48206768a7534e55bcpng.png"
                 size="large"
                 shape="square"/>
    </div>
    <el-form :model="form" class="el-form">
      <el-form-item label="">
        <el-input v-model="form.name" placeholder="用户名"></el-input>
      </el-form-item>
      <el-form-item label="">
        <el-input v-model="form.pwd" placeholder="密码"></el-input>
      </el-form-item>
    </el-form>
    <div class="confirm">
      <el-button type="success" default>登录/注册</el-button>
    </div>
    <div class="forget">
      <span>忘记密码</span>
    </div>
  </div>
</template>

<script>
import {reactive} from "vue";

const form =reactive({
  name: '',
  pwd: ''
})

export default {
  name: "BoardBox",
  data() {
    return {
      form: form
    }
  }
}
</script>

<style scoped>
.board_box {
  width: 300px;
  height: 260px;
  border: 1px solid rebeccapurple;
  border-radius: 2%;
  margin: 0 auto;
  background-color: rgba(20, 55, 87, 0.67);
}

.board_box span {
  color: #42b983;
}

.el-form {
  width: 220px;
  margin: 0 auto;
}

.header_img {
  margin: 20px 0;
}
.confirm {
  margin: 22px 0 0 0;
}

.forget span{
  color: #515965;
  font-size: 12px;
  float: right;
  margin: 0 9px 0 0;
}
</style>