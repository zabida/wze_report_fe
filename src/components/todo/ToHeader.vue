<template>
  <div>
    <el-input type="text"
              placeholder="请输入你的任务"
              :value="cont"
              @click.enter="add"></el-input>
  </div>
</template>

<script>
export default {
  name: "ToHeader",
  props: {
    cont: {
      type: String,
      default: ""
    }
  },
  methods: {
    add(){

    }
  }
}
</script>

<style scoped>

</style>