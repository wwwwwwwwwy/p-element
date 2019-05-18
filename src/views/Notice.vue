<template>
  <div>
    <el-button :plain="true" @click="successful">成功</el-button>
    <el-button :plain="true" @click="fail">错误</el-button>
  </div>
</template>

<script>
export default {
  methods: {
    successful() {
      this.$message({
        message: "恭喜你，这是一条成功消息",
        type: "success"
      });
    },
    fail() {
      this.$message.error("错了哦，这是一条错误消息");
    }
  }
};
</script>

