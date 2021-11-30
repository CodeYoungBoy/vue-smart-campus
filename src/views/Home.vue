<template>
  <div class="home">
     <el-button type="text" @click="open">点击打开</el-button>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
    methods: {
      open() {
        this.$alert('每天开心', '嘿嘿', {
          confirmButtonText: '确定',
          callback: action => {
            this.$message({
              type: 'info',
              message: `action: ${ action }`
            });
          }
        });
      }
    }
  }
</script>
