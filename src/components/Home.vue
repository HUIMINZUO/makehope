<template>
  <div>
    <el-button type="info" @click="logout">退出此账号</el-button>
  </div>
</template>

<script>
export default {
  methods: {
    logout () {
      window.seeionStorage.clear()
      this.$router.push('/login')
    }
  }
}
</script>

<style lang="less" scoped>

</style>
