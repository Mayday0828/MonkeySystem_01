<template>
  <el-table :data="tableData">
    <el-table-column prop="date" label="日期" width="140">
    </el-table-column>
    <el-table-column prop="name" label="姓名" width="120">
    </el-table-column>
    <el-table-column prop="address" label="地址">
    </el-table-column>
  </el-table>
</template>

<script>
export default {
  name: "Main",
  data() {
    const item = {
      date: '2016-05-02',
      name: '莫燕华',
      address: ' 梧州学院a12 '
    };
    return {
      tableData: Array(10).fill(item)
    }
  }
}
</script>

<style scoped>

</style>
