<template>
  <div id="page1">
    <el-table :data="tableData" style="width: 100%">
      <el-table-column prop="date" label="Date" />
      <el-table-column prop="name" label="Name" />
      <el-table-column prop="address" label="Address" />
    </el-table>
  </div>
</template>
<script>
export default {
  name: 'todoPage',
  data() {
    return {
      list: [],
      loading: false,
      finished: false,
      refreshing: false,
      count: '0',
      tableData: [
        {
          date: '2016-05-03',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        },
        {
          date: '2016-05-02',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        },
        {
          date: '2016-05-04',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        },
        {
          date: '2016-05-01',
          name: 'Tom',
          address: 'No. 189, Grove St, Los Angeles'
        }
      ]
    }
  },
  setup() {},
  created() {}
}
</script>
<style scoped>
#page1 {
  height: 100%;
  width: 100%;
  position: absolute;
}
</style>
