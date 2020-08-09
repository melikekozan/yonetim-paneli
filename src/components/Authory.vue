<template>
  <div class="card mb-3">
    <div class="card-header">
      <i class="el-icon-user"></i>
      YETKİLERİ
      <i style="float:right;" class="el-icon-circle-check"></i>
      <i style="float:right; margin-right:5px" class="el-icon-edit-outline"></i>
    </div>
    <div class="card-body">
      <el-collapse>
        <el-collapse-item>
          <template slot="title">
            <el-checkbox
              :indeterminate="isIndeterminate"
              v-model="checkAll"
              @change="handleCheckAllChange"
            >Check all</el-checkbox>
          </template>
          <div style="margin: 15px 0;"></div>
          <hr />
          <el-checkbox-group v-model="checkedCities" @change="handleCheckedCitiesChange">
            <el-checkbox v-for="city in cities" :label="city" :key="city">{{city}}</el-checkbox>
          </el-checkbox-group>
        </el-collapse-item>
      </el-collapse>
    </div>
  </div>
</template>

<script>
const Options = [
  "Shangggggghai",
  "Beijggggging",
  "Guanggggzhou",
  "Shegggnzhen",
];
export default {
  data() {
    return {
      checkAll: false,
      checkedCities: ["Shanghai", "Beijing"],
      cities: Options,
      isIndeterminate: true,
    };
  },
  methods: {
    handleCheckAllChange(val) {
      this.checkedCities = val ? Options : [];
      this.isIndeterminate = false;
    },
    handleCheckedCitiesChange(value) {
      let checkedCount = value.length;
      this.checkAll = checkedCount === this.cities.length;
      this.isIndeterminate =
        checkedCount > 0 && checkedCount < this.cities.length;
    },
  },
};
</script>

<style>
.card {
  margin-right: 8px;
  border-style: solid;
  border-color: #73c4be;
}
.card-header {
  color: #529991;
  background-color: #d2fafa;
  font-size: 14px;
  font-weight: bold;
  font-family: Verdana, Tahoma, sans-serif;
}
.card-header i {
  font-size: 17px;
}
</style>